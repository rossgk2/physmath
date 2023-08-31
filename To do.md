Advice for learning math
- when doing calculations, don't try to do too much in your head. write out each step on paper. this will help you make less mistakes. for example, something I always do is take an extra step to distribute negative signs when expanding polynomial expressions such as $x^2 + 3 - (x - 3)^2$. I would write $x^2 + 3 - (x - 3)^2 = x^2 + 3 - (x^2 - 6x + 9) = x^2 + 3 - x^2 + 6x - 9 = 6x - 6$. some people might skip writing out the second to last equation, but I always do it. 
- Build on your own knowledge. This is most relevant when some later concept requires you to make use of a convention regarding an earlier concept. I advise you to investigate what the later concept would look like if a different convention was the norm. Then choose, or come up with, a convention that you think is most intuitive.
- I personally learn by organizing information. I read stuff from a textbook, and then reorganize it into a way that I think is more natural (since textbooks often present information in slightly unnatural ways). When reading unsatisfyingly organized information, doing this is a good way to learn.
- When you're reading something that is satisfyingly organized, I advise learning by writing down the most important definitions and facts you come across as you read. See if you can boil everything important down into a list of bullet points.

Precalc
- possibly add section that summarizes things you learn in algebra
  - notation for multiplication: $\times, \cdot$, and $()$
  - you "solve equations" by doing the same operation to both sides of the equation 
  - "FOIL" and why it works  
- add note on why precalc matters: gives you a foundation for modeling phenomena. so is inherently useful even if you don't learn calc afterwards.
- add remark that " $f = f(x)$ " is bad but don't make it more complicated than that
- add explanation of "FOIL" and remark that you shouldn't rely on a mnemonic such as "FOIL"

Calculus

- attribute prime notation to Lagrange, not Newton 
- explain Leibniz notation by doing these things in some order:
  - maybe remark that $f(g)$ is better notation than $f \circ g$ for calculus purposes. then could state chain rule in prime notation: $\Big(g(f)'\Big)(x) = \Big(g'(f)\Big)(x) f'(x)$
  - The following shouldn't need to be a definition, but no one actually interprets the notation $\frac{df(x)}{dx}$ in this way, so we are forced to do so: $\frac{df(g(x))}{dg(x)} := f'(g(x))$. Also define $\frac{df}{dg} := x \mapsto \frac{df(g(x))}{dg(x)} = f'(g)$.
  - The notation $\frac{df}{dg} := f' \circ g$ is appealing because it allows for a nice statement of the chain rule as $\frac{d(g \circ f)}{dx} = \frac{dg}{df} \frac{df}{dx}$, but it is also problematic because since $(f^{-1})' = \frac{1}{df/df^{-1}}$ involves the notation $\frac{df}{df^{-1}}$, which does not behave as expected: we have $\frac{1}{df^{-1}/df} = \frac{1}{(f^{-1})' \circ f} \neq f' \circ f^{-1} = \frac{df}{df^{-1}}$. Interpreting $\frac{df}{df^{-1}}$ in a sensible way requires a extra layer of interpetation that's probably not worth it.
- $\int f(g) \frac{dg}{dx} = \int f \text{ } dg$ has two uses. When read left to right it formalizes the notion of canceling differentials. When read right to left it provides a way to change variables.
  - rename this theorem to something other than "change of variables theorem"- maybe "canceling differentials in the integrand" 
- swapping of limit variable theorem. if $f(x) \rightarrow L$ as $x \rightarrow p$ then $\lim\_{x \rightarrow p} g(f(x)) = \lim\_{f \rightarrow L} g(f)$. that is, if $\lim\_{x \rightarrow p} f(x) = L$ then $\lim\_{x \rightarrow p} g(f(x)) = \lim\_{f \rightarrow L} g(f)$.
  - might even be used to prove chain rule
- "you can indeed take the derivative of a derivative"; velocity, acceleration, jerk
- add derivative of polynomials after linearity of deriv: polynomials are important because $f'' = \text{const}$ implies $f'$ and $f$ are polynomaials. $\frac{d}{dx}:P\_n \rightarrow P\_{n - 1}$ and $\int:P\_n \rightarrow P\_{n + 1}$. 
- change deriv of inverse deriv rule to use chain rule
- definite integrals with change of variables theorem- bounds change

Multivariable calculus
- Come up with an algorithm that, given a bounded volume $V \subseteq \mathbb{R}^n$ and an order of integration $\sigma \in S_n$, determines the bounding functions $\int_V dV = \ell_1, ..., \ell_n$ and $u_1, ..., u_n$ such that $\int\_{\ell\_{\sigma(n)}}^{u\_{\sigma(n)}} \int\_{\ell\_{\sigma(n - 1)}(x\_{\sigma(n - 1)})}^{u\_{\sigma(n - 1)}(x\_{\sigma(n - 1)})} ... \int\_{\ell\_{\sigma(2)}(x\_{\sigma(2)}, x\_{\sigma(3)} ..., x\_{\sigma(n - 1)})}^{u\_{\sigma(2)}(x\_{\sigma(2)}, x\_{\sigma(3)} ..., x\_{\sigma(n - 1)})} \int\_{\ell\_{\sigma(2)}(x\_{\sigma(1)}, x\_{\sigma(2)}, x\_{\sigma(3)} ..., x\_{\sigma(n - 1)})}^{u\_{\sigma(2)}(x\_{\sigma(1)}, x\_{\sigma(2)}, x\_{\sigma(3)} ..., x\_{\sigma(n - 1)})} dx\_{\sigma(1)} dx\_{\sigma(2)} ... dx\_{\sigma(n - 1)} dx\_{\sigma(n)}$. This will involve investigating the hypotheses we need to assume about $V$ in order to make coming up with a reasonable algorithm possible. The algorithm will have to account for the fact that the output bounds may be piecewise functions for some orders of integration and non-piecewise functions for others.

Logic
- $P \implies Q$ and $P \iff Q$ are short for $(P \implies Q) \cong T$ and $(P \iff Q) \cong T$

Linear algebra
- Never say "let $E^* = {\phi^{\mathbf{e}\_i}}$ be the induced dual basis to $E$; this is redundant in light of the defn $\phi^{\mathbf{v}} := \mathbf{F}(\mathbf{v})$, where $\mathbf{F}(\mathbf{e}\_i) = \phi^{\mathbf{e}\_i}$ in the motivated intro chapter
- Edit discussion of vectors at beginning of chapter to discuss the following... There is circularity on the intuitive level between the notions of "point" and "vector". We can resolve this circularity on a formal level by defining each of "point" and "vector" in more primitive terms. Though, there is a circularity between the intuitive ideas of "point" and "vector" that will always persist.
  - Suppose we attempt to make "vector" the primitive concept on top of which we define "point". We may attempt to define a "point" to be a sum of vectors cooresponding to the directions of the coordinate axes. But a geometric understanding what a "sum" of vectors is requires the notion that adding a vector to a \textit{point} produces another \textit{point} (the sum of vectors $\mathbf{v}\_1 + \mathbf{v}\_2$ is understood as being the \textit{point} that is achieved by the sum $(\mathbf{p} + \mathbf{v}\_1) + \mathbf{v}\_2$r). We see our attempted deinition of "point" relies on the notion of "point", and is thus circular.
  - Suppose we attempt to make "point" the primitive concept on top of which we define "vector". We may attempt to define a "vector" to be a difference of points. But a geometric understanding of what a difference of points requires a notion of "vector" (the difference of points $\mathbf{p}\_2 - \mathbf{p}\_1$ is understood as being the difference between the \textit{vectors} $(\mathbf{p}\_2 - \mathbf{q})$ and $(\mathbf{p}\_1 - \mathbf{q})$, where $\mathbf{q}$ is any point). We see our attempted deinition of "vector" relies on the notion of "vector", and is thus circular.
- replace span(v_1, ..., v_k) with span({v_1, ..., v_k})
- graphically emphasize that closure under addition and scalar multiplication are the most important vector space axioms
- finish converting matrices section into setting of linear functions K^n -> K^m
- finish systems of linear equations section

Dual spaces
- instead of defining dual basis to be maps represented by $\mathfrak{e}\_1^\top, …, \mathfrak{e}\_n^\top$, first define unnatural isomorphism $\mathbf{F}:K^n \rightarrow K^{1 \times n}$ sending $\mathbf{v} \mapsto \mathbf{v}^\top$ and then define dual basis to be the maps represented by $\mathbf{F}(\mathfrak{e}\_1), …, \mathbf{F}(\mathfrak{e}\_n)$.
- add remark about using the unnatural isomorphism $\mathbf{F}$ to think about elements of dual space as (being represented by) row vectors

Recent physics and tensor stuff (8/25/23)
- $\frac{dy}{dx}$ and Oscar Cunningham's [dividing by a vector](https://oscarcunningham.com/4/dividing-by-a-vector/) blog post
- electromagnetic induction
- evidence for electric charges
- technical stuff
  - fix the theorem "Change of coordinates for tangent vectors in terms of basis vectors of $T\_{\mathbf{p}}(M)$" so that $\mathbf{x}(\mathbf{p})$ appears instead of $\mathbf{p}$ where necessary, and so that a result for general tangent vectors- not just basis tangent vectors- is stated
  - Add physics versions of manifold arguments to book
    - $\{\partial_i\}\_{i = 1}^n$ is a basis for $T\_{\mathbf{p}}(M)$: show $\frac{d}{dt} = \frac{dx^\mu}{dt} \partial_\mu$, where $x^\mu = (\mathbf{x} \circ \mathbf{r})^\mu$, where $\mathbf{r}:M \rightarrow \mathbb{R}$ is a curve on $M$ and $t$ is thought of as parameterizing $\mathbf{r}$
    - Change of basis for tangent vectors from fact that unprimed and primed coordinates represent same vector (this proof supresses the map that changes coordinates)
    - add a remark about the abuse of notation in which $dx^{\mu'}$ is written rather than $dx'^\mu$. (at least, I think some people do this)
- read more about GR
- review D'Alembert's principle (and maybe read about analytical mechanics, which focuses on scalar quantities), 
- review the Euler-Lagrange equation and Lagrangian mechanics
- read the Wikipedia article that derives SR's four-momentum by using the Euler-Lagrange equation; then review four-momentum stuff, including $E = mc^2$!
- review orientation of manifolds
- review Stokes' theorem
- How does thinking about the differential as a pushforward relate to changing coordinates?
- finish understanding coordinate representation of Hodge dual
  - this will involve reviewing identities involving Levi-Civita symbol and generalized Kronecker delta
- read about the covariant derivative from Carroll's GR text
- do a concrete example of computing $T_{\mathbf{p}}(M)$ for $M$ that's the image of a smooth function $\mathbb{R}^2 \rightarrow \mathbb{R}$

Tensors
- condense second pushforward and pullback section; then take results involving pushforwards/pullbacks out of determinant section and merge all pushforward/pullback stuff to one section that goes at the end of the exterior powers chapter
- Hodge dual edits
  - To derive Hodge dual $\perp$, define $\frac{\perp \omega}{h(\omega, \omega)}$ on a $k$-wedge $\omega$ of orthonormal basis vectors and extend with seeming-multilinearity and alternatingness. Then determine coordinates of $\frac{\perp \eta}{h(\eta, \eta)}$ relative to this basis, and compute $\omega \wedge (\perp \eta)$. Result should be $\text{vol}$.
  -  if $\dim(V) = n$, can the Hodge dual $\*:\Lambda^k(V) \rightarrow \Lambda^{n - k}(V)$ be deduced from $\*:\Lambda^{n - 1}(V) \rightarrow (V)$?
  -  Investigate the relationship between interior multiplication and the Hodge dual.
- replace quotes "" with parentheses () when enclosing statements
- make sure that indexing convention is followed after def of covariance and contravariance (just moved it to dual spaces section)
- mention the term "staggered indices" after defn of coordinates of tensor
- move proof of \[\vv\]\_E^i = \phi^{\ee_i}(\vv) and (\[\phi\]\_{E^\*})\_i = \phi(\ee_i) to after derivation of induced dual basis
- CTRL-F "alternization" and replace with "antisymmetrization" when necessary; the alt operator should probably be renamed to be asym
- Is it best to think of $\widetilde{\otimes}$, $\widetilde{\wedge}$ as induced, or as special cases of $\otimes$, $\wedge$ for different spaces? (by "special cases", I refer to fact that $\widetilde{\otimes}$ and $\widetilde{\wedge}$ are the versions of $\otimes$ and $\wedge$ on certain spaces, specifically, the versions that satisfy $(\phi^1 \otimes ... \otimes \phi^n)(\mathbf{e}\_1, ..., \mathbf{e}\_n) = \prod_i \phi^i(\mathbf{e}\_i)$, and a sim. characterizing property)
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
  
