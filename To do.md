advice for learning math
- when doing calculations, don't try to do too much in your head. write out each step on paper. this will help you make less mistakes. for example, something I always do is take an extra step to distribute negative signs when expanding polynomial expressions such as $x^2 + 3 - (x - 3)^2$. I would write $x^2 + 3 - (x - 3)^2 = x^2 + 3 - (x^2 - 6x + 9) = x^2 + 3 - x^2 + 6x - 9 = 6x - 6$. some people might skip writing out the second to last equation, but I always do it. 
- Build on your own knowledge. This is most relevant when some later concept requires you to make use of a convention regarding an earlier concept. I advise you to investigate what the later concept would look like if a different convention was the norm. Then choose, or come up with, a convention that you think is most intuitive.
- I personally learn by organizing information. I read stuff from a textbook, and then reorganize it into a way that I think is more natural (since textbooks often present information in slightly unnatural ways). When reading unsatisfyingly organized information, doing this is a good way to learn.
- When you're reading something that is satisfyingly organized, I advise learning by writing down the most important definitions and facts you come across as you read. See if you can boil everything important down into a list of bullet points.

precalc
- possibly add section that summarizes things you learn in algebra
  - notation for multiplication: $\times, \cdot$, and $()$
  - you "solve equations" by doing the same operation to both sides of the equation 
  - "FOIL" and why it works  
- add note on why precalc matters: gives you a foundation for modeling phenomena. so is inherently useful even if you don't learn calc afterwards.
- add remark that " $f = f(x)$ " is bad but don't make it more complicated than that
- add explanation of "FOIL" and remark that you shouldn't rely on a mnemonic such as "FOIL"

calc

- attribute prime notation to Lagrange, not Newton 

- explain Leibniz notation by doing these things in some order:
  - remark that $f(g)$ is better notation than $f \circ g$ for calculus purposes
  - state chain rule in prime notation: $\Big(g(f)'\Big)(x) = \Big(g'(f)\Big)(x) f'(x)$
  - The following shouldn't need to be a definition, but no one actually interprets the notation $\frac{df(x)}{dx}$ in this way, so we are forced to do so: $\frac{df(g(x))}{dg(x)} := f'(g(x))$. Also define $\frac{df}{dg} := x \mapsto \frac{df(g(x))}{dg(x)} = f'(g)$.
  - Should formalize the notion of "preferred letters" for single variable functions because this convention is used in the general context of a function $f$ accepting $n$ real numbers. (For such a multivariable function $f$, we often associate the $i$th argument with the symbol $x_i$. This association makes notation like $\frac{\partial f}{\partial x_i}$ unambiguous. In formalizing this convention it could be useful to use the operator $\partial_i$ to denote the taking of the $i$th partial derivative.)
  - now chain rule can be stated in a slightly better way (one way in terms of functions eval'ed on inputs and one way in terms of functions)
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
- $P \implies Q$ and $P \iff Q$ are short for $(P \implies Q) \cong T$ and $(P \iff Q) \cong T$

linear algebra
- replace span(v_1, ..., v_k) with span({v_1, ..., v_k})
- graphically emphasize that closure under addition and scalar multiplication are the most important vector space axioms
- finish converting matrices section into setting of linear functions K^n -> K^m
- finish systems of linear equations section

tensors
- Hodge dual edits   
  - There really is no good motivation for coming up with defn of Hodge dual on $\omega = \mathbf{u}\_{i_1} \wedge ... \wedge \mathbf{u}\_{i_k}$, since the factor $\langle \omega, \omega \rangle$ has to be included. And that factor must be there. (Somehow earlier I thought it didn't).
  - Use instead the derivation at https://www.homotopico.com/page2/.
- replace quotes "" with parentheses () when enclosing statements
- make sure that indexing convention is followed after def of covariance and contravariance (just moved it to dual spaces section)
- mention the term "staggered indices" after defn of coordinates of tensor
- move proof of \[\vv\]\_E^i = \phi^{\ee_i}(\vv) and (\[\phi\]\_{E^\*})\_i = \phi(\ee_i) to after derivation of induced dual basis
- CTRL-F "alternization" and replace with "antisymmetrization" when necessary; the alt operator should probably be renamed to be asym
- if dim(V) = n, can the Hodge dual \*:Lambda^k V -> Lambda^(n - k) V be deduced from \*:Lambda^{n - 1} V -> V?
- Investigate the relationship between interior multiplication and the Hodge dual.
- Is it best to think of \totimes, \twedge as induced, or as special cases of \otimes, \wedge for different spaces? (by "special cases", I refer to fact that \totimes and \twedge are the versions of \otimes and \wedge on certain spaces, specifically, the versions that satisfy (phi^1 \otimes ... \otimes \phi^n)(e_1, ..., e_n) = prod_i phi^i(e_i), and a sim. characterizing property)
- Bases used for orientation on a vector space with metric tensor should often be assumed to be orthonormal, because we can always use Gram-Schmidt to get at an underlying orthonormal basis
- A choice of basis on a vector space does in some sense induce a dual basis, maybe? A choice of basis induces the "dot product" on the vector space, and that has an associated musical isomorphism. (I suspect that the "dot product" may only be a metric tensor when the basis is orthonormal, though...)
- After the "orthonormal <=> self-dual" remark, use the notation $\huu_1, ..., \huu_n$ for bases when speaking of a induced dual basis rather than the notation $\ee_1, ..., \ee_n$?
- The purpose of T \wedge S := \alt(T \otimes S) isn't to demonstrate a model for \wedge, but to show that V^{\wedge k} \subseteq T^k_0(V)
- improve section on orientation forms if necessary (add footnote on the terminology "volume form", maybe even use it myself; add a section "volume forms and the metric tensor"

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

add a github section about "beatufiul interpretations"
- algebra lets us see shifting a line left is the same as shifting it down
- function-input duality. Let $X$ and $Y$ be sets and let $X^\*$ denote the set of functions from $X$ to $Y$. Then when for $x \in X$ and $f \in X^\*$ we consider the expression $f(x)$, we can of course consider $f$ to be a function, but we can also consider $x$ to be a function that acts on $f$; formally, we mean that for every $x \in X$ there is a function $F_x \in X^{\*\*}$ that acts on $f \in X^\*$ by $F_x(f) = f(x)$.  
- in physics, interpreting velocity to be a function of position helps complete the derivation for the kinetic eneryg formula
- interpreting functions as derivatives and vice-versa to leverage the chain rule


deprecated (don't actually implement this)
- introduce the notion of preferred letters.
    - $\bar{S}$ := the preferred letter of S
    - define " $f$ is a function of $x$ " <=> $\bar{f} = x$. later, define " $f$ is a function of $x_1, ..., x_n$ " <=> similar notation 
    - $S_T$ := function mapping quantities represented by $T$ to quantities represented by $S$
  - introduce the notion of conflating $S$ with $\bar{S}$
  - note: may seem weird, but if $\bar{g} = f$ and $\bar{f} = x$, then $\widebar{\frac{dg}{df}} = x$. in particular this means $\frac{dg}{df} \frac{df}{dx}$ makes sense, since $\frac{dg}{df}$ and $\frac{df}{dx}$ both have a preferred letter of x. 
  - now chain rule can be stated in the way we want: if $\bar{g} = f$ and $\bar{f} = x$ then $\frac{dg}{dx} = \frac{dg}{df} \frac{df}{dx}$
  
