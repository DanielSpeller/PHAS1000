#Calclulus_and_Functions #PHAS1000 #Y1 
**Maclaurin series**
Often, we can simplify calculations by approximating complicated functions by suitable polynomials. For some arbitrary function $f$ , let’s assume that we can do this by writing
$$f(x)=\sum^{\infty}_{k=0}c_{k}x^k=c_{0}+c_{1}x+c_{2}x^2\dots$$
where $c_{k}$ are a set of coefficients. Evaluating the function at $x = 0$ gives
$$f(0)=\sum^{\infty}_{k=0}=c_{k}0^k=c_{0}+0+0\dots$$
so we can identify the coefficient $c_0$ with $f (0)$. Differentiating $f$ with respect to  $x$, and then evaluating at $0$, we find
$$f'(x)=\sum^{\infty}_{k=0}=kc_{k}x^{k-1}=0+c_{1}+2c_{k}x+\dots$$
$$f'(0)=\sum^{\infty}_{k=0}=kc_{k}0^{k-1}=0+c_{1}+0+\dots$$
and we can identify $c_1$ with $f ′(0)$. Similarly, looking at the $k^{th}$ derivative of the $k^{th}$ term of the series
$$\frac{d^k}{dx^k}c_{k}x^k=\frac{d^{k-1}}{dx^{k-1}}kc_{k}x^{k-1}$$
$$=\frac{d^{k-2}}{dx^{k-2}}k(k-1)c_{k}x^{k-2}$$
$$\dots$$
$$= k(k-1)(k-2)\dots 3 \cdot 2 \cdot 1 \cdot c_{k}x^0$$
$$=k!c_{k}$$
All previous terms in the series will have vanished after this many derivatives, and all higher terms will still have some power of x associated with them. So evaluating the $k^{th}$ derivative at $x = 0$ returns $k!c_{k}$. In general, then, we have
$$c_{k}=\frac{f^{k}(0)}{k!}$$
where $f (k)$ denotes the $k^{th}$ derivative.  Substituting this back into the original power series, we find
$$f(x)=\sum^\infty_{k=0} \frac{f^k(0)}{k!}x^k$$**Proofs of convergence**
$$\sum^{\infty}_{n=0}u_{n}=u_{0}+u_{1}+u_{2}+\dots$$
If the series converges then 
$$u_{n}\to{0},n\to \infty$$
However , if
$$u_{n}\to{0},n\to \infty$$
the series does not necessarily converge 

If 
$$\lim_{ n \to \infty } \left( \frac{u_{n+1}}{u_{n}} \right)<1$$
 , the series converges

If 
$$\lim_{ n \to \infty } \left( \frac{u_{n+1}}{u_{n}} \right)>1$$
, the series diverges

The last two statements constitute d’Alembert’s ratio test. The test is inconclusive if the limit is exactly 1.

**Taylor series**
In general, if we wish to expand a function $f$ about the point $a$, we let
$$f(x)=\sum_{k=0}^{\infty}c_{k}(x-a)^k$$
and following the same steps as in the derivation of the Maclaurin series, we can show that
$$c_{k}=\frac{f^{k}(a)}{k!}$$
so,
$$f(x)=\sum^\infty_{k=0} \frac{f^k(a)}{k!}(x-a)^k$$
This more general function expansion is called a Taylor series, of which the Maclaurin series is just a special case.

[[Taylor Series PPT.pdf]]
