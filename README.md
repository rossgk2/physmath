# Physically-inspired math

My ultimate ambition for this "physmath" project is to develop a series of textbooks that *satisfyingly* explain a lot of physically-inspired math, starting from precalculus. Here's the rough syllabus:

- Thoughts on how to learn math (2 pages)
- Precalculus
- Calculus
- Single variable calculus
- Linear algebra teaser: dot product, cross product, and equation of a plane
- Multivariable calculus
- Logic and proof-writing
- Linear algebra
- Differential geometry
  - Tensors
  - Basic topology
  - Calculus on manifolds with tensors

I love every single one of these topics just as much as the culmination that is differential geometry, so I won't be offended if you decide to stop halfway through the calculus textbook or something like that. (It's not like I'll know if you do so!). 

And let's be real- if even five or so people read some of just my precalculus texbook and come away with new insights, I'll be happy. Seriously. Precalculus is one of math's subjects that is treated the worst!

# Towards actually satisfyingly explained math

Okay, but what makes "satisfying" math? I certainty want to avoid the "that's the way it is" attitude that you find so-often in high school math classrooms. But beyond that, I want to improve upon the "conjecture and prove" pedagogy that traditional approaches to higher mathematics overuse/abuse. In "conjecture and prove", the proposed truths (conjectures) are always plausible enough, but also always seem to be somewhat unmotivated, somewhat popping out of thin air. It's true that some ideas are radical enough perspective shifts that they can only be perceived as coming out of the blue, but most ideas can be related to a previously known network of ideas in a natural way that lends to their discovery.

Satisfyingly explained math is essentially the opposite of "conjecture and prove" math. Heuristically, a concept has been satisfactiorly explained if, in the scenario where you are restricted from access to any outside resources- like textbooks, notes, the Internet- you can retrace the concept's story and eventually reobtain all the details. **My textbooks aim to present a plausible avenue by which every mathematical concept they cover could be discovered.**

I admit, it is unlikely that a single person would be able to independently make all of these natural discoveries *for the first time*. But, a textbook can take care of the first time for you! After you have digested the material, you will be left with that memorable path of discovery for a long time.

## Specifics of pedagogy

Here are some more specifics on the failings of "conjecture and prove" and on what exactly I think of as satisfingly explained math.

The "conjecture and prove" pedagogy is defined by the following three failings:

- Concept definitions are often given no real motivation (the "motivation" is often historical- e.g. "the Greeks noticed this", "Euler noticed that").
  - In particular, the following malpractice regarding definitions is often followed. Textbooks often first define what it means for an object to have a certain property P, and then prove a theorem that states that having this certain property is equivalent to another statement S. This approach is malpractice because the reader likely pauses after the definition of property P to ask themselves, "Why are objects with propety P important?". Of course, if the reader is experienced, then they will know to expect that the answer to the question is coming soon- they will get their answer when they read a theorem that equates property P to the statement S- but if the reader is not experienced, then they may feel immediately lost. A much better way to present the same information is to switch the order of theorem and definition. That is: first derive via a natural investigation that statement S is true for objects that have a certain property, and then define an object to have property P if statement S is true. This provides automatic motivation for why objects with property P are important.
- The proposed truths (conjectures) are always plausible enough, but also lack motivation and seem to somewhat pop out of thin air.
- The proofs of truths are unenlightening, since they are treated as tasks to be ticked off of a to-do list rather than as lines of reasoning to be deeply understood.

Satisfyingly explained math is diametrically opposed to "conjecture and prove" math, and recognizes these three core tenets:

- Concept definitions must be given real motivation.
  - As is suggested in the corresponding sub-bullet-point above, a common way to motivate a definition is to prove, *before* the definition is stated, that the definition describes objects for which a meaningful statement holds. 
- Conjectures must be given real motivation. The best way to motivate a conjecture is to derive it (prove that it is true) by starting from previously known ideas and following a natural/plausible avenue of investigation.
- A good proof is simultaneously a proof and an explanation. That is, a good proof is a self-explaining proof.

If you combine the above three core tenets, you realize that satisfyingly explained math is characterized by the following *two* tenets:

- Concept definitions must be given real motivation.
- Whenever possible, truths should be derived via self-explaining proof instead via conjecture and proof. If you must use the conjecture-prove approach, make sure the conjecture has real motivation and that the proof is self-explaining.

### The dreaded "efficency" pedagogy

Another mathematical philosophy to be desperately avoided, even worse than "conjecture and prove", is what I call the "efficiency" pedagogy. The "efficiency" pedagogy goes as follows. Suppose we are describing a mathematical object, and that we know that the object has a natural intuitive property N exactly whenever the object also has a wacky and esoteric property W.

If we are presenting this material, what we *should* do is first define property N, since it is more intuitive, and then prove that property W follows from property N, *even if* it is easier to prove that property N follows from property W. It doesn't make sense to start with W- no one would dream up W in the first place without discovering N first!

The "efficiency" pedagogy doesn't care about this. If it is easier to prove that N follows from W, then the "efficiency" pedagogy will first state W and then prove N.

If you think about it, the "efficency" pedagogy isn't actually that efficent. Sure, it may take less logic to prove W => N than it does to prove N => W, but, if one is to truly *understand* the material, they will eventually have to prove N => W. It is better to start with N => W, as it eliminates unnecessary confusion and elucidates what is really going on.

A prime example of the "efficiency" pedagogy is the typical way in which e, e^x, and ln(x) are defined. One common approach in to define ln(x) with a definite integral, then define x -> e^x to be the inverse function to ln, and then define e := e^1. This approach establishes all relevant facts about e^x and ln(x), including the fact d/dx e^x = e^x, but it does not give an intuition for why the facts are true. All of the other common approaches have this same issue. (The one pedagogically correct approach is to notice that d/dx b^x = c_b * b^x for some constant c_b, and then define e to be the b for which c_b = 1. Thus d/dx e^x = e^x. We also define ln to be the inverse function to x -> e^x. You can the details in my calculus textbook).

## Particular sins of traditional math

Here's a list of sins that traditional math commits (a good amount of these sins are resultant from the "conjecture and prove" philosophy, but not all of them are):

- Not stopping to pause at the fact that pi being a constant, and not a function of a circle's radius, is actually kinda cool.
- In the precalculus setting, saying things such as "let y = f(x)", and thereby conflating functions (e.g. f) with functions evaluated on inputs (e.g. f(x)).
- Not explaning why definitions involving exponents such as b^x := 1/b^{-x} are natural.
- Glossing over the fact that the nth root of x is *different notation* for x^{1/n}, and instead insinuating that one could somehow prove that the nth root of x is equal to x^{1/n}. (Both denote the evaluation of the inverse function of x -> x^n at x).
- Not giving memorable intuition for the facts log_b(x y) = log_b(x) + log_b(y) and log_b(x^y) = y log(x). At best, the traditional approach relies on the proof that begins by taking ln of both sides of b^{x + y} = b^x + b^y. (That's the best *proof* there is, but it isn't the best intution).
- Making students memorize rules that describe the end behavior of rational functions rather than emphasizing the practice of deriving these rules with limits at infinity. 
- Stating the chain rule by using the vague notion of differentiation with respect to "u = g(x)", rather than defining df/dg := f' compose g and stating the chain rule as d(f compose g)/dx = df/dg dg/dx.
- Defining e and the natural logarithm by "jumping to the conclusion" and skipping all relevant motivation. (Typically, ln will defined to be a definite integral of 1/x, and e will either be defined to be a limit, or as the result of a convergent series, or as ln^{-1}(1)).
- Proving that FTC 1 => FTC 2 rather than FTC 2 => FTC 1. (FTC 2, the second fundamental theorem of calculus, is actually more intuitive than FTC 1, the first fundamental theorem of calculus).
- Not explaining why the following two definitions of the dot product are equivalent: (1) v . w := |v||w|cos(theta) and (2) v . w := v_1 w_1 + ... + v_n w_n. When traditional math *does* explain, it uses the unintuitive law of cosines to do so.
- Insisting that you have to make weird shapes with your hand to apply the right hand rule rather than explaining the concept of orientation, and how orientation (and therefore the direction of the cross product) flips when the counterclockwise angle from one vector to another exceeds pi.
- Not making it clear that the right hand rule is a *convention* that is tied to the convention of depicting coordinate systems in the "right handed way" (e_1 = xhat as into the page, e_2 = yhat as horizontal, e_3 = zhat as up).
- Presenting the change of variables formula for integrals to be a chance discovery instead of a natural mirroring of the chain rule.
- Not explaining why "canceling differentials" works when performing separation of variables.
- Not explaining that the implication operator only takes on its English-langauge meaning when you use it inside a "for all" quantifier.
- Presenting the correspondence between linear transformations and matrices to be a coincidence.
- Emphasizing thinking of matrices as grids of numbers rather than as lists of vectors.
- Favoring the "multilinear function" definition of tensor over the "multilinear element" definition of tensor.
- Not explaining how each and every one of the topological space axioms generalizes the topological properties of the real numbers.
- Not mentioning the closure operator characterization of topologies.
