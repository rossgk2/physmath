# physmath
A collection of works on math underlied by spatial/physical intuition.

# End goal
My ultimate ambition for this project is to develop a series of textbooks that 

the reader from knowing zero precalculus to knowing some fairly advanced differential geometry.

- Precalculus
- Calculus
-- Single variable calculus
-- Multivariable calculus
--- Linear algebra teaser: dot product, cross product, and equation of a plane 
- Logic and proof-writing
- Linear algebra
- Differential geometry
-- Tensors
-- Basic topology
-- Calculus on manifolds with tensors

In general, I feel that traditional math uses the "conjecture and prove" formula way too much. With "conjecture and prove", the conjectures are always plausable, but always seem to pop out of thin air to some degree.

A much better philosophy that my textbooks abide by is "tell a story".

There are many, many instances in which I feel traditional approaches mar the beauty of math. 

Here are some, off the top of my head. Traditional math...
- Defines e and the natural logarithm by "jumping to the conclusion" and skipping all motivation. (Typically, ln will defined to be a definite integral of 1/x, and e will either be defined to be a limit, or as the result of a convergent series, or as ln^{-1}(1)).
- Won't give memorable intuition for ln(xy) = ln(x) + ln(y) and ln(x^y) = y log(x), and, at best, will rely on the proof that begins by taking ln of both sides of e^{x + y} = e^x + e^y.
- Won't explain why the following two definitions of the dot product are equivalent: (1) v . w := |v||w|cos(theta) and (2) v . w := v_1 w_1 + ... + v_n w_n. When traditional math *does* explain, it uses the unintuitive law of cosines to do so.
- Will insist that you have to make weird shapes with your hand to apply the right hand rule, rather than explaining the concept of orientation, and how orientation (and therefore the direction of the cross product) flips when the counterclockwise angle from one vector to another exceeds pi.
- Won't make it clear that the right hand rule is a *convention* that is tied to the convention of depicting coordinate systems in the "right handed way" (e_1 = xhat as into the page, e_2 = yhat as horizontal, e_3 = zhat as up)
- Will present the change of variables formula for integrals to be a chance discovery instead of a natural mirroring of the chain rule.
- Won't explain why "canceling differentials" works when performing separation of variables.
- Will present the correspondence between linear transformations and matrices to be a coeincidence.
