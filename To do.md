precalc
- add note on why precalc matters: gives you a foundation for modeling phenomena. so is inherently useful even if you don't learn calc afterwards.
- add remark that "f = f(x)" is bad but don't make it more complicated than that

calc

- edit entire calc book to incorporate "improved physicist's Leibniz notation"; i.e. Leibniz notation that makes use of the notion of preferred letters and functions such as S_T
  - add note that "S = T" means "sym(S) = sym(T)"
  - will still need to include defn. df/dx := f' or f(x) where the choice is determined by context 

- swapping of limit variable theorem. if f(x) - > L as x -> p then lim_{x -> p} g(f(x)) = lim\_{f -> L} g(f). that is, if lim\_{x -> p} f(x) = L then if lim\_{x -> p} g(f(x)) = lim\_{f -> L} g(f)
  - might even be used to prove chain rule
- "you can indeed take the derivative of a derivative"; velocity, acceleration, jerk
- add derivative of polynomials after linearity of deriv: polynomials are important because x'' = const implies x' and x are polynomaials. d/dx:P_n -> P\_{n - 1} and int:P_n -> P\_{n + 1} 
- change deriv of inverse deriv rule to use chain rule
- definite integrals with change of variables theorem- bounds change
- phi linear function rmk. add that "linear elts are a gen of vectors"

logic
- "P => Q" and "P <=> Q" are short for "(P => Q) =~ T" and "(P <=> Q) =~ T"

linear algebra

- discussion of R^n and finite dimensional vector spaces over R before vector space over field defn
- simplify matrix derivations so that they correspond to linear functions K^n -> K^m

github readme
- add to list: better FTC 2 => FTC 1 than other way. but is it even common practice to do FTC 1 => FTC 2?
- sometimes, theorems are not stated in the most memorable way
  - Cauchy-Schwarz
  - rank-nullity
  - John Lee's two theorems about derivations did not explicitly say that set of derivations = set of directional derivative functions
  - sometimes, things that fall naturally out of a definition are presented as theorems (e.g. matrices, matrix vector prod, matrix matrix prod)
- work and energy in physics as an example of confusingly presented defns
- interpretations are cool
  - exponential functions as using any base
  - consider g(x) = x - h, f(x) = x. can consider g as being result of shifting f down, or as shifting f to the right. reveals that down is the same as right for positively sloped lines
  - velocity as a function of position. a = dv/dx dx/dt
  - functions as derivatives, derivatives as functions
- physics
  - N2 => N1, so N2, N3 are the only Newton's laws that are necessary

  - if the center c of a frame is not accelerating, c'' = 0, then the force mx'' on an object in the frame includes  "fictitious" contribution. this proves that "laws of physics in all nonaccelerating (i.e. inertial) frames are the same". no need to take as axiom
