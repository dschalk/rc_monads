<script>
    import async from "$lib/images/Screenshot_async.png";
    import asyncIdpng from "$lib/images/Screenshot_asyncId.png";
    import { merge_ssr_styles } from "svelte/internal";
    import { fade } from "svelte/transition";
    import Layout from "../+layout.svelte";
    import Header from "../Header.svelte";

    var log = console.log;
    function ret() {}

    function M1(x) {
        return function go(func) {
            if (func === ret) return x;
            x = asyncId(x).then((v) => func(v));
            return go;
        };
    }

    var M1Code = `function M1 (x) {
  return function go (func) {
      if (func === ret) return x;
      x = asyncId(x).then(v => func(v));
      return go;
  }
}

WHERE async function asyncId (x) {return x};`;

    var monad = `function M (x) {
    return function go (func) {
        if (func === ret) return x
        x = func(x);
        return go;
  }
}`;

    var asyncIdCode = `async function asyncId (x) {return x};

(A) var m2 = M1(3);
console.log(m2(ret));  // 3

(B) asyncId(m2(ret)).then(v=>console.log(v));  // 3

(C) asyncId(asyncId(asyncId(m2(ret))))
.then(v=>console.log(v));  // 3`;

    async function asyncId(x) {
        return x;
    }
    async function wait(t) {
        setTimeout(function () {}), t * 1000;
    }
    var m1 = M1(2);
    var m2 = M1(
        new Promise((resolve, reject) => {
            setTimeout(() => {
                resolve(2);
            }, 1500);
        })
    );

    var mpow = (y) => async (x) => asyncId(x).then((v) => (x = v ** y));
    var msqrt = (x) => asyncId(x).then((v) => (x = Math.sqrt(v)));
    var mMult = (y) => (x) => asyncId(x).then((v) => (x = v * y));
    var madd = (y) => async (x) => {
        await wait(2);
        return x + y;
    };

    m1(mpow(10))(Math.sqrt)(madd(52))(mMult(2))((a) => a * 2)(async (x) => {
        await wait(2);
        return x / 8;
    });

    m2(mpow(10))(Math.sqrt)(madd(52))(mMult(2))((a) => a * 2)(async (x) => {
        await wait(2);
        return x / 8;
    });

    console.log("m1(ret) is", m1(ret));
    console.log("m2(ret) is", m2(ret));
</script>


<svelte:head>
    <title
        >Asynchronous and Synchronous Values Handled by Slightly Modified
        RC_Monads</title
    >
</svelte:head>
<br />
<div>
    **************************************************************************
</div>
<div
    style="font-family: Times New Roman; text-align:center; font-size: 32px;"
    transition:fade
>
    <br />

    A modified version of rc_monads handles both <br> sychronous and asynchronous functions.
</div>
<br />
<p>This is the function that creates rc_monads, as described in the <a href = "../">Introduction</a>
<pre>{monad}</pre>
<p>
    Here's the modification in which the function go() makes x  promises and synchronous code'
</p>
<pre>{M1Code}</pre>
<p>
    AsyncId makes promises out of non-promises and has no effect on promises as
    shown below.
</p>
<pre>{asyncIdCode}</pre>
<p>
    "A" (above) shows that m2(ret) == 3. Calling asyncId on m2(ret) in "B"
    returned a promise whose fulfullment value is 3. The Part B Promise is both
    the argument and the return value of asyncId in "C".
</p>

<style>
    img {
        width: 100%;
        height: 100%;
    }
    h3 {
        color: turquoise;
    }
    
    a {
        margin: 1px;
        color: coral;
        padding: 1px ;
        text-decoration: none;
        text-shadow: none;
	    box-shadow: 0px 0px 4px 0px rgb(255, 255, 0);
    }
    p {
        text-indent: 0px;
    }
</style>
