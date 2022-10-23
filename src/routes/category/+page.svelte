<script>

	import { binding_callbacks, element } from 'svelte/internal';
import { fade } from 'svelte/transition';

var monoidDef = `A set S equipped with a binary operation S × S → S, which we will 
denote •, is a monoid if it satisfies the following two axioms:

Associativity
For all a, b and c in S, the equation (a • b) • c = a • (b • c) holds.

Identity element
There exists an element e in S such that for every element a in S, 
the equalities e • a = a and a • e = a hold.`;

var rc_addText = `var rc_add = x => y => {
    let a = x(ret);
    let b = y(ret);
    return M(a+b);
}`;

var increment = `const m1 = M(3);
const add_1 = rc_add(M(1));

m1 = add_1(m1)
console.log(m1(ret))   // 4
m1 = add_1(m1)
console.log(m1(ret))   // 5
m1 = add_1(m1)
console.log(m1(ret));  // 6`;

var add = `
const m2 = M(5);
const m3 = M(13);
var c = rc_add(m1)(m2);
c(ret)  // 21
const m4 = M(21);
rc_add(rc_add(m2)(m3))(m4)  // 39`;

var add_1 = `
var add_1 = rc_add(M(1));
m1 = add_1(m1)
console.log(m1(ret))   // 4
m1 = add_1(m1)
console.log(m1(ret))   // 5
m1 = add_1(m1)
console.log(m1(ret));  // 6`;

var add_2 = `
var m2 = M(5);
var m3 = M(13);
var c = rc_add(m1)(m2);
c(ret)  // 21
var m4 = M(21);
log(rc_add(rc_add(m2)(m3))(m4)(ret))  // 39
log(rc_add(m2)(rc_add(m3)(m4))(ret))  // 39`;

</script>

<style>
    a {
        margin: 1px;
        color: coral;
        padding: 1px ;
        text-decoration: none;
        text-shadow: none;
        size: 22px;
	    box-shadow: 0px 0px 4px 0px rgb(255, 255, 0);
    }
</style>

<svelte:head>
	<title>Some Observations In the Realm of Category Theory</title>
</svelte:head>
<br />
<div>**************************************************************************</div>
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />
    Monoids, Monads, and RC_Monads <br>Some Random Observation
    </div>
<p>DISCLAIMER: I'm not providing many rigorous proofs here, just musing a little about the behavior of sets of rc_monads. After getting my bachelor's degree in chemistry from Indiana University, I got a master's degree in mathematics. That was forty-three years ago. I got a doctor of jurisprudence degree from the Indiana University Schoold of Law and passed the Indiana bar examination, both in 1990. I never intended to pursue a career in mathematics and I am far from being an expert in the field.</p>
<p> Let &#8469; be the set of all non-negative numbers; i.e., the natural numbers and 0. let &#8473; be the set of rc_monads containing elements of &#8469. Addition on N forms a monoid because (1) it has a left and right identity element, 0, and (2) &#8473 commutes; i.e., rc_add(j,rc_add(k,n)) = rc_add(rc_add(j,k),n) for all j, k, and n in &#8469;. Here's the definition of a monoid:</p>
<pre>{monoidDef}</pre>
<div>References: <a href="https://en.wikipedia.org/wiki/Monoid">monoid in Wikipedia</a>
    <span>, </span>
    <a href = "https://ncatlab.org/nlab/show/monoid#AsAOneObjectCategory">monoid in nLab</a>   
</div>
<p>Let f be a mapping from &#8469; into &#8473 defined by f: (k,+) -> (M(k),rc_add) for all k in &#8469;. This isn't standard notation, but I think you get my drift. f preserves structure and is, therefore, a functor.</p> 
<pre>{rc_addText}</pre>
<p>rc_add maps &#8473 onto itself. The set rc_add( (M(j),M(k) ) for all j and k in &#8469 is nothing more or less than &#8473. If k is greater than j, rc_add(M(j),M(k)) = rc_add(M(j+1),M(k-1)) = ... = rc_add(M(j+k),M(0)). Sets don't contain duplicates so the equivalence stated above stands.</p>

<p>So much for sets, what about the category consisting of all mappings (a/k/a "morphisms" and "arrows") rc_add(M(j),M(k)) -> M(j+k) for all j and k in &#8469. Arrows from multiple pairs to the same destination are allowed. This isn't a set. Functors that map categories onto themselves are called "endofunctors.</p>

<p> Now back to the question: Is rc_add(j,k) for some elements j and k of &#8469 an instance of a monoid in a category of endofunctors? I sense that we are close, but not quite there. Enough for now.     </p>       

<h3>Some Definitions and Examples</h3>

<span class="tao">Partial application of rc_add yields functions that add specific amounts to any other rc_monad in the set of rc_monads holding integers in &#8469. Here's the definition of add_1 and its application to m1 three times:</span>
<br>
<pre>{increment}</pre>
<br>
<div>Next we'll add two rc_monads and then demonstrate that rc_add is associative.</div>
<pre>{add_2}</pre>
<h3>Monads</h3>
<span class="tao">A monad is a monoid in a category of endofunctors. Does &#8473 exist in a category of endofunctors?  It seems to. rc_add on &#8473 obeys the monad laws, which are left identity, right identity, and associativity. That will be reassuring should I ever use interacting rc_monads and need to lift (a strict functional programming language term) &#8473 into the the category of mulltiplication over the natural numbers. Categories seem a lot like types when thought of this way. </span>







