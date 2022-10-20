


<script>
	// @ts-ignore

	import { get_root_for_style, merge_ssr_styles } from 'svelte/internal';
	//	import { onMount } from "svelte";
	import { fade } from 'svelte/transition';
    import Page from './score/+page.svelte';
	// import Index from "./index.svelte";
	// import { top } from './stores.js';
	// import { userName } from './stores.js';
    var m3 = M(3);
    var s = ret; 

var m2 = M(32);	
var m0 = M([]);
		m2 = M(m2(s));
function nav2 () {
	let n = m2(ret)[5];
	m2(ar => m0(ret).slice(-n)[0])
	update();
	sfunc();
	return m2;
}
var QQ;
$: QQ = m2(ret)[6];

function back () {
	if (ar3.length < 3) return;
	var o = ar3.pop();
	m2(ar => o);
	update();
	sfunc();
	return m2;
}

function splash (a) {
    m2 = M(a);
	// console.log("In splash @@@ m2(ret) is",m0(ret).join(", "));
    update();
    sfunc();
}

 /*   m0(ar => ar.concat(clone([m2(ret)])));
	m2(v => [[1,2,3,4], [], ["+"], [], [0], [], [0], []]);
    m0(ar => ar.concat(clone([m2(ret)])));
	m2(v => [[0,7,0,7], [], ["+"], [], [0], [], [0], []]);
    m0(ar => ar.concat(clone([m2(ret)]))); */
console.log("**********************************************");
console.log("At the top. m0(ret) is", m0(ret));
console.log("**********************************************");

	var PIN, WINNERS;
	var WIN = 1000.0;
	var FIN = 1001.0;
	var FINAL;
	var millisec = 0;
	var seconds = 0;
	var timer;
	var d2;
	var startStop = 'Start';
	var value;
	var d2 = '';
	var A,
		B,
		C,
		D,
		AA,
		BB,
		CC,
		DD,
		EE,
		FF,
		GG,
		HH = 'wait';
	var N = 0;
	var l = console.log;
	var b0 = 'none';
	var b1 = 'none';
	var b2 = 'none';
	var b3 = 'none';
	var index;
	var b4 = 'none';
	var b5 = 'none';
	var b6 = 'none';
	var b7 = 'none';
	var s = ret;
	var AA;
	var BB;
	var CC;
	var DD;
	var EEE = 'awaiting selection';
	var FF;
	var WW;
	var XX;
	var YY;
	var ZZ;
	var SCORE;
	$: SCORE = [0];
	var ZYXW;
	var WXYZ;

	var zeros = () => {
		var arr2 = [
			[0,0,0,0],
			[],
			['+'],
			[],
			[0],
			[],
			0,
			[]
		]};

function ret () {};

function M (x) {
    return function go (func) {
        if (func === ret) return x
        else x = func(x);
        return go;
  }
}

	var runRoller = (b = 0) => {
		var arr2 = [
			[0,0,0,0],
			[],
			['+'],
			[],
			[b],
			[],
			0,
			[]
		];
		m2 = M(arr2);
		updateRoll(m2);
		resettimer();
		resettimer();
	};

	var runRoll;
	runRoll = (b) => {
		var arr = [
			[
				Math.floor(Math.random() * 6) + 1,
				Math.floor(Math.random() * 6) + 1,
				Math.floor(Math.random() * 12) + 1,
				Math.floor(Math.random() * 20) + 1
			],
			[],
			['+'],
			[],
			[b],
			[1],
			1,
			[]
		];
		QQ = 1;
		m2(a => arr);
		ar3 = [clone(arr),clone(arr), clone(arr)];
		EEE = 'yet to be selected';
		updateRoll(m2);
		// m2(fu);
		if (tog) display();
	    console.log("In runRoll. m0(ret) is", m0(ret));
		return m2;
	};
	var Z = '';
	$: Z;
	var x;
	function updateRoll(m) {
		console.log('In updateRoll. m(s) is', m(s));
		AA = m(s)[0][0];
		BB = m(s)[0][1];
		CC = m(s)[0][2];
		DD = m(s)[0][3];

		WW = m(s)[1][0];
		XX = m(s)[1][1];
		YY = m(s)[1][2];
		ZZ = m(s)[1][3];
		EE = m(s)[2];
		FF = m(s)[3];
		SCORE = m(s)[4];
		b0 = b1 = b2 = b3 = 'inline';
		b4 = b5 = b6 = b7 = 'none';
	}
	function sfunc() {
		b0 = b1 = b2 = b3 = b4 = b5 = b6 = b7 = 'none';
		if (AA != (undefined && 0)) b0 = 'inline';
		if (BB != (undefined && 0)) b1 = 'inline';
		if (CC != (undefined && 0)) b2 = 'inline';
		if (DD != (undefined && 0)) b3 = 'inline';
		if (WW != (undefined && 0)) b4 = 'inline';
		if (XX != (undefined && 0)) b5 = 'inline';
		if (YY != (undefined && 0)) b6 = 'inline';
		if (ZZ != (undefined && 0)) b7 = 'inline';
	}

	var update = function update() {
		AA = m2(s)[0][0];
		BB = m2(s)[0][1];
		CC = m2(s)[0][2];
		DD = m2(s)[0][3];
		EE = m2(s)[2];
		FF = m2(s)[3];
		SCORE = m2(s)[4];
		WW = m2(s)[1][0];
		XX = m2(s)[1][1];
		YY = m2(s)[1][2];
		ZZ = m2(s)[1][3];
	};
/*
	$: AA = m2(s)[0][0];
	$: BB = m2(s)[0][1];
	$: CC = m2(s)[0][2];
	$: DD = m2(s)[0][3];
	$: EE = m2(s)[2];
	$: FF = m2(s)[3];
	$: SCORE = m2(s)[4];
	$: WW = m2(s)[1][0];
	$: XX = m2(s)[1][1];
	$: YY = m2(s)[1][2];
	$: ZZ = m2(s)[1][3];    */

	var ZWIN = '';
	var mon3 = M([1, 2, 3, 4]);

	function calc(aa, bb, c) {
		var a = parseInt(aa, 10);
		var b = parseInt(bb, 10);
		if (c === '+') return a + b;
		else if (c === '*') return a * b;
		else if (c === '-') return a - b;
		else if (c === '/') return a / b;
		else if (c === '@') return ' ' + a + b;
		else return 'fubar';
	}

	function g(ar) {
		var x = ar.pop() ** 3;
		ar.unshift(x);
		return ar;
	}

	function g2(ar) {
		return ar.flatMap((v) => (v + 1) ** 3);
	}
	function g3(ar) {
		return ar.flatMap((v) => Math.round(v ** (1 / 3)));
	}

	function clone(x) {
		return JSON.parse(JSON.stringify(x));
	}

	function test() {
        console.log("m2(ret)is", m2(ret));
        console.log("ar3 is", ar3);
	}

	var ar3;
	$: ar3 = [];
	$: ar3.length;
	
	function fu(a) {
		var result;
		var a1;

		if (a[1].length === 2 && a[2].length === 1) {
			a1 = a[1];
			result = calc(a[1][0], a[1][1], a[2][0]);
			a[0].push(result);
			a[3].push(result);
			a[1] = [];
			a[5][0] += 1;
			a[6] += 1;
			m2(v => a);
		}

		if (a[1].length === 3) {
			a[0].push(a[1].pop());
		}

		if (result == 20 && intersection(a1, a[3]).length > 0) {
			if (a[4][0] == 2) {
				resettimer();
				PIN = FIN;
				if (FIN < WIN) WIN = FIN;
				ZWIN = 'You win! Your score is ';
				WINNERS = WIN;
				// top.set([WIN]);
				setTimeout(() => runRoller(),4000);
				// setTimeout(() => a[4][0] = 0,8000);
			} else {
				var aint = parseInt(a[4], 10);
				aint += 1;
				Z = '           Your score increased to ' + aint;
				runRoll(aint);
			}
			setTimeout(() => (Z = ZWIN = ''), 8000);
		}
		ar3.push(clone(a));
		ar3 = ar3;
		update();
		sfunc();
		return m2(s);
	}

	var fmon = (f) => (x) => x(f);
	var reset = (x) => [1, 2, 3, 4];

	var click0 = (a) => {
		a[1].push(a[0][0]);
		a[0].shift();
		m2 = M(a);
		m2(fu);
		// sfunc();
	};

	/* var click0 = a => {
    a[1].push(a[0].splice(0,1)[0]);
    m2 = M(a);

}; */

	var click1 = (a) => {
		a[1].push(a[0].splice(1, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	var click2 = (a) => {
		a[1].push(a[0].splice(2, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	var click3 = (a) => {
		a[1].push(a[0].splice(3, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	function clic0(m) {
		EEE = 'add';
		m[2] = '+';
		m2 = M(m);
	}

	$: clic1 = (m) => {
		EEE = 'subtract';
		m[2] = '-';
		m2 = M(m);
	};

	function clic2(m) {
		EEE = 'multiply';
		m[2] = '*';
		m2 = M(m);
	}

	function clic3(m) {
		EEE = 'divide';
		m[2] = '/';
		m2 = M(m);
	}

	function clic4(m) {
		EEE = 'concat';
		m[2] = '@';
		m2 = M(m);
	}

	$: Z = Z;

	var m4 = M(3.1415926535);
	var cube = (x) => x ** 3;
	var pow = n => x => x**n;
	var square = x => x*x; 
	var add = (n) => (x) => 1 * x + 1 * n;
	var mult = (n) => (x) => x * n;
	var reset2 = (n) => (x) => (x = n);

	function squareFu() {
		m4 = m4(square);
	}
	function cubeFu() {
		m4 = m4(cube);
	}

	function divFraction(x) {
		var y = x.split('/');
		if (y.length > 1) {
			return y[0] / y[1];
		} else {
			return y[0];
		}
	}
	var powFu = function powFu(e) {
		var p = divFraction(e.target.value);
		if (e.keyCode == 13) {
			m4 = m4(pow(p));
		}
	};

	var addFu = function addFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(add(e.target.value));
		}
	};

	var multFu = function multFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(mult(divFraction(e.target.value)));
		}
	};

	var resetFu = function resetFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(reset2(divFraction(e.target.value)));
		}
	};

	function intersection(a, b) {
		return a.filter((x) => b.includes(x));
	}

	$: XO = m2(s);

	var tog = true;

	var display = function display() {
		tog = false;
		if (millisec >= 9) {
			millisec = 0;
			seconds += 1;
		} else millisec += 1;
		d2 = seconds + '.' + millisec;
		timer = setTimeout(() => display(), 100);
	};

	function starttimer() {
		if (timer > 0) {
			return;
		}
		display();
	}
	function stoptimer() {
		clearTimeout(timer);
		timer = 0;
	}

	function startstoptimer() {
		if (startStop === 'Start') startStop = 'Stop';
		else startStop = 'Start';
		if (timer > 0) {
			clearTimeout(timer);
			timer = 0;
		} else {
			display();
		}
	}

	function resettimer() {
		clearTimeout(timer);
		FIN = d2;
		var temp = m2(s);
		temp[4] = [0];
		m2 = M(temp);
		millisec = 0;
		seconds = 0;
		d2 = seconds + '.' + millisec;
		tog = true;
	}

	var fuDem = `function fu (a) {                                    // fu
  a[5].push(clone(a));
  a[7].push(clone(a)); // All game states for use in "Back" and "Forward."
  a[6][0] += 1;
    // a[1].push(a[0].pop());
  var result;
  SCORE = a[4];
  var a1;
  if (a[1].length === 2 && a[2].length === 1)   {
    a1 = a[1];
    result = calc(a[1][0], a[1][1],a[2][0]);
    a[0].push(result);
    a[3].push(result);
    a[1] = [];
    m2 = M(a);
  }

  if (a[1].length === 3) {
    a[0].push(a[1].pop());
  }

  if (result == 20 && intersection(a1, a[3]).length > 0) {
      if (SCORE === 4) {
          ZWIN = "You win! "
          a[4][0] = 0;
          runRoll(0);
      }
      else {
          var aint = parseInt(a[4][0], 10);
          aint += 1;
          Z = "           Your score increased to " + aint;
          runRoll(aint);
      }
      setTimeout(() => Z = ZWIN = "", 3000);
  }
  update();
  sfunc();
  return m2(s);
};

var update = () => { // The button displays will correspond to the values in m2.
  AA = m2(s)[0][0];
  BB = m2(s)[0][1];
  CC = m2(s)[0][2];
  DD = m2(s)[0][3];
  EE = m2(s)[2];
  FF = m2(s)[3];
  SCORE = m2(s)[4];
  WW = m2(s)[1][0];
  XX = m2(s)[1][1];
  YY = m2(s)[1][2];
  ZZ = m2(s)[1][3];
}

function sfunc () {
    b0 = b1 = b2 = b3 = b4 = b5 = b6 = b7 = "none"; // All button displays controlled by b's disappear.
    if (AA != (undefined && 0)) b0 = "inline"; // Next, selected buttons are diplayed.
    if (BB != (undefined && 0)) b1 = "inline";
    if (CC != (undefined && 0)) b2 = "inline";
    if (DD != (undefined && 0)) b3 = "inline";
    if (WW != (undefined && 0)) b4 = "inline";
    if (XX != (undefined && 0)) b5 = "inline";
    if (YY != (undefined && 0)) b6 = "inline";
    if (ZZ != (undefined && 0)) b7 = "inline";
}`;


var monad = `function M (x) {
    return function go (func) {
        if (func === ret) return x
        else x = func(x);
        return go;
  };
};

function ret () {};`

var monad3 = `var mon3 = M([1,2,3,4]);
    function g(ar) {
        var x = (ar.pop())**3;
        ar.unshift(x);
        return ar;
};
function g2 (ar) {return (ar.flatMap(v => (v+1)**3))};
function g3 (ar) {return (ar.flatMap(v => Math.round(v**(1/3))))};`;

	var simple = `var s = 'stop';
var m4 = M(3);   // creates a new monad named "m4".
var cube = x => x**3;
var square = x => x*x;
var pow = n => x => x**n;
var add = n => x => 1*x + 1*n;
var mult = n => x => x * n;
var reset2 = n => x => x = n;`;

	var runR = `runRoll = x => {
    m2 = M([ [Math.floor(Math.random()*6) + 1, 
	Math.floor(Math.random()*6) + 1, 
	Math.floor(Math.random()*12) + 1, 
	Math.floor(Math.random()*20) + 1], [], [], [], [x] ]);
    updateRoll();
    EEE = "yet to be selected";
    XO = m2('stop');
    AR = [];
    index = 0;
}

const updateRoll = () => {
  AA = m2(s)[0][0];
  BB = m2(s)[0][1];
  CC = m2(s)[0][2];
  DD = m2(s)[0][3];

  WW = m2(s)[1][0];
  XX = m2(s)[1][1];
  YY = m2(s)[1][2];
  ZZ = m2(s)[1][3];
  EE = m2(s)[2];
  FF = m2(s)[3];
  SCORE = m2(s)[4];
  b0 = b1 = b2 = b3 = "inline";
  b4 = b5 = b6 = b7 = 'none';
};`;

	var clickFuncs = `var click0 = a => {
    a[1].push(a[0][0])
    a[0].shift();
    m2 = M(a);
    m2(fu);
    // sfunc();
};

var click1 = a => {
    a[1].push(a[0].splice(1,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

var click2 = a => {
    a[1].push(a[0].splice(2,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

var click3 = a => {
    a[1].push(a[0].splice(3,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

function clic0 (m) {
  EEE = "add";
  m[2] = "+";
  m2 = M(m) ;
}

$: clic1 = m => {
  EEE = "subtract";
  m[2] = "-";
  m2 = M(m) ;
}

function clic2 (m) {
  EEE = "multiply";
  m[2] = "*";
  m2 = M(m) ;
}

function clic3 (m) {
  EEE = "divide";
  m[2] = "/";
  m2 = M(m) ;
}

function clic4 (m) {
  EEE = "concat";
  m[2] = "@"
  m2 = M(m);
};`;

	var putBack = `if (a[1].length === 3) {
    a[0].push(a[1].pop());  // Returns a clicked third number.
  };`;

	var fuFuncs = `function squareFu () {m4 = m4(square)};
function cubeFu () {m4 = m4(cube)};

function divFraction (x) {
    var y = x.split('/');
    if(y.length > 1){
        return (y[0] / y[1])
    }
    else{
        return y[0];
    }
}

var powFu = function powFu (e) {
    var p = divFraction(e.target.value);
    if (e.keyCode == 13) {
        m4 = m4(pow(p));
    }
};

var addFu = function addFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(add(e.target.value));
    };
  };

var multFu = function multFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(mult(divFraction(e.target.value)))};
};

var resetFu = function resetFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(reset2(divFraction(e.target.value)))
    };
};`;

	var example0 = `var mon = M(2); // mon's value is the anonymous function returned by M.     `;

	var example3 = `var mon = M(2);
mon(v=>v**4)(v=>v+5)(v=>v*2);`;
	// The value of x can be obtained later
	var example4 = `mon(ret);  // 42
mon(v => v*v);`;
	// And later:
	var example5 = `mon(ret);  // 1764`;

	var oldMonad = `function M (x) {
    return function go (func) {
        if (typeof func === "function") {
            x = func(x);
            return go;
        }
        else if (func === "stop") return x;
    }
};`;

	var buttons = `<button style = "display: {b0}" on:click = {() => m2(click0)}>{AA}</button>
<button style = "display: {b1}" on:click = {() => m2(click1)}>{BB}</button>
<button style = "display: {b2}" on:click = {() => m2(click2)}>{CC}</button>
<button style = "display: {b3}" on:click = {() => m2(click3)}>{DD}</button>

<span style = "margin-left: 8%; font-size: 22px">The operator is {m2(s)[2]}</span>

<br><br>
<button on:click = {() => m2(clic0)}>add</button>
<button on:click = {() => m2(clic1)}>subtract</button>
<button on:click = {() => m2(clic2)}>multiply</button>
<button on:click = {() => m2(clic3)}>divide</button>
<button on:click = {() => m2(clic4)}>concat</button>
`;
	var backDem = `back = a => {
    if (a[5].length < 1) {
      m2 = M(a);
      console.log("You're already all the way back")
      return;
    }
    else {
        var b = a[5][a[5].length - 1];
        b[7] = a[7];
        m2 = M(b);
        update();
        sfunc();
    }
};

var forward;
$: forward = a => {
    var index = a[6][0];
    if (a[5].length === a[7].length) {
        console.log("Already at the top");
        m2 = M(a);
        return;
    }
    else {
        var b = a[7][index + 1];
        b[7] = a[7];
        m2 = M(b);
        update();
        sfunc();
    }
};`;

var example2 = `var m3 = M(3);
var m4 = M(m3(s));
m3(v => v + 3);
m4(v => v + 4);

log("m3(s) * m4(s) is", m3(s) * m4(s))

m3(s) * m4(s) is 42`;

	var example6 = `M(2)(v=>v+1)(v=>v*2)(v=>v*7)(s) // 42`;

	var async = `var asyncMult = a => async b => {
    var d;
    if (!(b instanceof Promise)) return a * b;
    else d = await b;
    return a * d;
}

var asyncAdd = a => async b => {
    var d;
    if (!(b instanceof Promise)) return a + b;
    else d = await b;
    return a + d;
}

m3(asyncAdd(4))(asyncMult(6))(s).then(v => log("The result is", v));  // The result is 42
m3(asyncAdd(8))(asyncMult(2))(s).then(v => log("Now we are at", v));  // Now we are at 100
m3(asyncAdd(-51))(asyncMult(6/7))(s).then(v => log("And back to", v)) // And back to 42 `;

var retCode = `function ret () {}`

	var bigMonad = `function Comp ( AR = [] )  {
  var f_, p, run;
  var ar = AR.slice();
  var x = ar.pop();
  return run = (function run (x) {
    if (x === null || x === NaN ||
      x === undefined) x = f_('stop').pop();
    if (x instanceof Filt) {
      var z = ar.pop();
      if (x.filt(z)) x = z; else ar = [];
    }
    else if (x instanceof Promise) x.then(y =>
      {if (y != undefined && typeof y !== "boolean"
        && y === y && y.name !== "f_" && y.name !== "stop" ) {
      ar.push(y);
      diffRender()
    }})
    else if (x != undefined && x === x && x !== false
      && x.name !== "f_" && x.name !== "stop" ) {
      ar.push(x);
      diffRender()
    };
    function f_ (func) {
      if (func === 'stop' || func === 'S') return ar;
      else if (func === 'finish' || func === 'F') return Object.freeze(ar);
      else if (typeof func !== "function") p = func;
      else if (x instanceof Promise) p = x.then(v => func(v));
      else p = func(x);
      return run(p);
    };
    return f_;
  })(x)
}`;

	var caution = `var s = ret;
var log = console.log;

function M(x) {
  return function go(func) {
    if (typeof func === "function") {
      x = func(x);
      return go;
    } else if (func === "stop") return x;
  }
};

var m3 = M(3);

m3(async a => await 888); // m3(s) will return a Promise with value 888.

m3(s).then(v => m3((z => v + 112)));
// m3(s) will return 1000 after the promise is fulfilled.

m3(s).then(v => setTimeout(() => console.log("m3(s) resolved is", v,), 2000));
// The promise is still pending, so the value of "v" is 888.

setTimeout(() => console.log("m3(s) is", m3(s)),0);
// This gets bumped to the bottom of the stack, behind (2).
// m3(s) is called after x has been updated to 1000.

// Result:
16:13:15.590 m3(s) is 1000
16:13:17.590 m3(s) resolved is 888
// Two seconds after "1000" appears in the console log, "888" is displayed.`;


var start = `m2 = M([ [ Math.floor(Math.random() * 6) + 1, 
           Math.floor(Math.random() * 6) + 1,
           Math.floor(Math.random() * 12) + 1, 
           Math.floor(Math.random() * 20) + 1 ], 
           [], ['+'], [], [0], [], [0], [] ]);`

var unit = `function unit (m,v){
    m(() => v)
    return m;
}

var m = M("Hello nurse");
unit(m,42);
m(ret)  // 42   `;

var rc_add_ex = `var rc_add = x => y => {
    let a = x(ret);
    let b = y(ret);
    return M(a+b);
}`

var rc_add_1_ex = `var add_1 = rc_add(M(1));

var m1 = M(3);
var a = add_1(m1)
log(a(ret))  // 4
var b = add_1(a)  
log(b(ret))  // 5
var c = add_1(b)
log(c(ret))  // 6`;



setTimeout(() => splash( [[1,,,], [], ["+"], [], [0], [], [0], []] ),500);
setTimeout(() => splash( [[0,,,], [], ["+"], [], [0], [], [0], []] ),1000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),1500);
/*  setTimeout(() => splash( [[4,4,4,4], [], ["+"], [], [0], [], [0], []] ),1500);
setTimeout(() => splash( [[3,3,3,3], [], ["+"], [], [0], [], [0], []] ),2000);
setTimeout(() => splash( [[2,2,2,2], [], ["+"], [], [0], [], [0], []] ),2500);
setTimeout(() => splash( [[1,1,1,1], [], ["+"], [], [0], [], [0], []] ),3000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),3500);
setTimeout(() => splash( [[8,8,8,8], [], ["+"], [], [0], [], [0], []] ),4000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),4500);  */

var id_ex =`const m1 = M(3);
const id = rc_add(M(0));
id(m1)(ret) === m1(ret) // true`

</script>

<style>
	pre {margin-left: 3%;}
</style>

<svelte:head>
	<title>The Solitaire Game of Score</title>
</svelte:head>
<br />
<div>**************************************************************************</div>
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />
Introduction To RC_Monads
    <br>
</div>
<p>This presentation explores the potential usefulness of recursive closures created by calling M(x) where, respectively, M and ret are:</p>  
<pre>{monad}</pre> 
<p>These recursive closures are called "rc_monads". Note: periods go outside of quotation marks surrounding function names, URLs, and any other text where a period could possibly cause ambiguity. </p>	
<p>The function returned by calling M(x) operates on functions that operate on x in M(x). There are no restrictions on what x can be; for example, it can be a primitive value, an objects, or telescoping copies of M(x). The value of x in the <a style = "margin-left:8px" href="./score">Solitaire Game of Score</a>, listed as "Score" in the menu (above), is an array of eight arrays. </p>
	
<p>M(x) can work anonymously or be named as in "const rcm = M(x)." In that case, rcm(some function) returns itself each time it executes, with one exception. It occurs when "some function" (above) is named "ret". What ret() does or doesn't do is of no consequence since it never gets called. The name "ret" causes x in M(x) to be returned instead of The rcm-M(x) closure remains available indefinitely for further action on x. 	</p>

<p>Encapsulation, Composition, and other features will be explained in detail on this Page. If you want to play the simulated solitaire dice game, made with x in M(x) being an array of eleven arrays, click <a style = "margin-left:8px" href="./score">Solitaire Game of Score</a>.	But please be sure to come back, especially if you write JavaScript code. I think you will be pleasantly surprised by the potential utility of rc_monads and if wrapping your head around what is going on takes some time, this will be a valuable learning experience. The possibilities latent in first-class functions are amazing and, once recognized, can result in code that is exceptionally concise, robust, and powerful	. </p>
<p>If you want to see JavaScript mimick the Haskell programming language, Google "javascript monads" and knock yourself out. I'm a Haskell programmer who gets great satisfaction from 	working with Haskell, but I'm not going to forego the amazing possibilities of JavaScript in order to make it purely functional, or to make it mimick the functions in the Haskell Prelude library as so many bloggers and YouTube presenters do.   </p>

<h2>Composition Using Anonymous RC_Monads</h2>
<p>Composition is jaw-droppingly simple. Just put M() (x === "undefine" // true) or M(x) for some other value of x in front of a series of functions.</p>
<span>Example:<span class = "pre"> M()(()=>2)(x=>x*3)(x=>x * Math.floor(7.3))(ret)</span>  // 42</span>
<br>
<span>Example:<span class = "pre"> M(2)(x=>x*3)(x=>x * Math.floor(7.3))(ret)</span>  // 42</span>
<p>The value of x goes from "undefined" to 2, 6, and finally 6 * 7 in the first example. The second example goes from 2 to 6 and then 6 * 7. In both cases, the un-named closure is subject to garbage collection.</p>
<p>Here comes one more example. It will be used to elucidate the value of named rc_monads in the next section.</p>
<span>Example:<span class = "pre"> M()(()=>2)(x=>x*3)(x=>x*Math.floor(7.3))(v=>v+58)(v=>Math.sqrt(v))(ret)</span>  // 10</span>
<br>
<h2>Maintaining Encapsulated State In Named RC_Monads</h2>
<p>We can define an rc_monad m and follow it with functions all on one line. m is still m after it has operated on functions that update x in the m-M(x) closure.</p>
<span class = "pre">let m = M(2)(x=>x*3)(x=>x * Math.floor(7.3))</span>
<span class="pre">m(ret) // 42</span>
<p>"m" and the instance of M holding the value 42 form a closure that, like all closures, is not subject to garbage collection. We can now compute "10" as in the anonymous example (above) without repeating the computation that yielded 42.</p>
<span class="pre">m(v=>v+58)(v=>Math.sqrt(v) </span>
<span class="pre">m(ret) // 10</span>
<br>

<h2>RC_Monads Can Be Objects In Categories</h2>
<p>Let C be the collection of all rc_monads holding positive integers and let rc_add (see below) be the basis for defining function mapping them to one another. </p>
<pre>{rc_add_ex}</pre>

<p>Here's the identity function on C:</p>
<pre>{id_ex}</pre>

<p>The integer held in an rc_monad can be mapped to the rc_monad holding the next integer sequentiall with rc_add, defined by partially applying rc_add to the rc_monad holding the number 1. </p>
<pre>{rc_add_1_ex}</pre>

<p>Here's a morphism from m5, where m5(ret) === 13 is true, to the rc_monad in C holding the number 21: <span class="pre">m5(v=>v+8). </span><span>I didn't need to give it a name.</span> <span class="pre">m5(v=>v+8) </span><span> is the object in C holding the number 21. C happens to be a monoid, but that's enough category theory for now.</p>


    <h2>Conclusion</h2>
<p>I use rc_monads to encapsulate and update state. I provided a non-rigorous glimpse of them behaving like objects in a category partly because it's fun to experiment and partly to justify characterizing rc_monads as monads. Members of the "functional programming" cargo cult, people who obsess on types, immutability, and pure functions without knowing when these features are helpful and when they are unnecessarily stifling, will probably consider me a heretic anyway, but I tried.</p> 
    
<p>To me, functional programming in JavaScript is using functions efficiently and creatively. Dividing applications into small modules makes it safe to take shortcuts that would otherwise be dangerous, such as using global variables and functions with side effects that alter them. When dynamic state has to be protected from mistakes by me, team members, or future maintainers, independent modules with immutable data, strict typing, and pure functions can provide confidence that malfunctions and hidden bugs won't appear. Another approach would be to use rc_monads in the midst of unfettered JavaScript or in independent, secure modules such as those described above.</p>    


<slot></slot>
