6#Calclulus_and_Functions #PHAS1000 #Y1 
Recall that a function is a map from one set to another, $f : A → B$. So far, we have been interested in functions from and to some subset of the real numbers, $f : R → R$. However, we can consider much more general functions than this. For example, the function $f : \mathbb R ^2 → \mathbb R, f (x, y) = x^2 + y$ maps two real inputs to a unique output. To see how this function behaves, consider firstly the function $f_{0} : \mathbb R → \mathbb R, f_{0}(x) = x^2$. We know this function well and can plot it on a graph. Now consider the similar function $f_{1}(x) = x^2 + 1$.  
This is just a translation of $f_{0}$. Similarly, we can define $f_{k}(x) = f_{0}(x) + k$ for any value of $k$ and have an intuitive understanding of this function. We can also draw plots of any of these functions for arbitrary values of $k$

If we depict the value of k on a separate y axis there are an infinite number of such curves, if we plot them all we build a two-dimensional surface as, and we have a visual representation of our function $f (x, y) = x^2 + y$ via the 3D graph $z = f (x, y)$

We approached this by considering quadratics in x with different values of y. This corresponds to looking at cross-sections of the full surface for constant values of y. We can show several cross-sections of the full surface that give back ordinary one-dimensional functions of the form $f_{k}(x)= x^2 + k$ for some constant value of $k$.  

For any of these functions, we could differentiate and find the slope of the cross-section:
$$\frac{df_{k}}{dx}=\frac{d(x^2+k)}{dx}=2x$$$$df(x,y)= \frac{\partial f}{\partial x}dx+\frac{\partial f}{\partial y}dy$$
Suppose $x$ and $y$ depend on some parameter, $t$. A small change in $t,dt$ gives
$$df= \frac{\partial f}{\partial x}\frac{dx}{dt}dt+\frac{\partial f}{\partial y}\frac{dy}{dt}dt$$
[[Partial Diffentiation.pdf]]
