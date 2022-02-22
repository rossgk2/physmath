advice for learning math
- when doing calculations, don't try to do too much in your head. write out each step on paper. this will help you make less mistakes. for example, something I always do is take an extra step to distribute negative signs when expanding polynomial expressions such as x^2 + 3 - (x - 3)^2. I would write x^2 + 3 - (x - 3)^2 = x^2 + 3 - (x^2 - 6x + 9) = x^2 + 3 - x^2 + 6x - 9 = 6x - 6. some people might skip writing out the second to last equation but I always do it. 
- Build on your own knowledge. This is most relevant when some later concept requires you to make use of a convention regarding an earlier concept. I advise you to investigate what the later concept would look like if a different convention was the norm. Then choose, or come up with, a convention that you think is most intuitive.
- I personally learn by organizing information. I read stuff from a textbook, and then reorganize it into a way that I think is more natural (since textbooks often present information in slightly unnatural ways). When reading unsatisfyingly organized information, doing this is a good way to learn.
- When you're reading something that is satisfyingly organized, I advise learning by writing down the most important definitions and facts you come across as you read. See if you can boil everything important down into a list of bullet points.

precalc
- add note on why precalc matters: gives you a foundation for modeling phenomena. so is inherently useful even if you don't learn calc afterwards.
- add remark that "f = f(x)" is bad but don't make it more complicated than that
- add explanation of "FOIL" and remark that you shouldn't rely on a mnemonic such as "FOIL"

calc

- attribute prime notation to Lagrange, not Newton 
- explain Leibniz notation by doing these things in some order:
  -- remark that f(g) is better notation than f \circ g for calculus purposes
  -- state chain rule in prime notation: g(f)' = g'(f) f'
  -- introduce the notion of preferred letters and the notation S_T := S(Sbar)(T),
  introduce the notion of conflating S with S_Sbar
  -- define df(g(x))/dg(x) := f'(g(x)). note, f(g(x)) = f(g)(x), so presumably df(g(x))/dx = d(f(g)(x))/dg(x). but in this last expression, we still don't know what having a function in the "denominator" means, so the definition is necessary. also define df(g)/dg := x -> df(g(x))/dg(x) = f'(g)
  -- note: may seem weird, but if gbar = f and fbar = x, then (dg/df)bar = x. in particular this means dg/df df/dx makes sense, since dg/df and df/dx both have a preferred letter of x. 
- int f(g) dg/dx = int f dg has two uses. when read left to right it formalizes the notion of canceling differentials. when read right to left it provides a way to change variables.
  - rename this theorem to something other than "change of variables theorem"- maybe "canceling differentials in the integrand"
    -- explain how variables are actually changed from g to x. 
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
