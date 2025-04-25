#Calclulus_and_Functions #PHAS1000 #Y1 
For a sine function with period L we can generalise a group of functions as $\sin\left(\frac{2\pi nx}{L}\right),\forall x\in \mathbb Z$

A sine function is defined as odd as $f(-x)=-f(x)$ and can be thought about as rotationally symmetric
A cosine function is defined as even as $f(-x)=f(x)$ and can be thought about as symmetry in reflection

Any [[Functions|function]] can be written as an even part and odd part
$$f_{e}(x)=\frac{f(x)+f(-x)}{2},f_{o}(x)=\frac{f(x)-f(-x)}{2},f(x)=f_{e}(x)+f_{o}(x)$$
A set of functions of period L is a vector space and can be written as a combinations of trigonometric functions
$$1,\sin\left(\frac{2\pi nx}{L}\right),\cos\left(\frac{2\pi nx}{L}\right)\forall n\geq 1$$
This relies of the trigonometric function being orthogonal. We can defined the inner product on space as functions as
$$<f\ |\ g> \ =\int_{domain}f^*(x)\ g(x) \ dx$$
Dirichlet conditions:
- Must be periodic
- Finite number of discontinuities per period
- Finite number of maxima and minima
- Absolutely integrable $\int^L_{0}|f(x)| \ dx<\infty$

$$f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}a_{n}\cos\left(\frac{2\pi nx}{L}\right)+\sum_{n=1}^{\infty}b_{n}\sin\left(\frac{2\pi nx}{L}\right)$$
[[Fourier Series PPT.pdf]]
