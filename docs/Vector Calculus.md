#Y1 #PHAS1000 #Calclulus_and_Functions 
In the definition above of the ordinary derivative, notice that the numerator is the difference of two numbers, $f (x + δx) − f (x)$. This is an operation that  we also know how to perform in the case of vectors. Suppose we have a vector that depends on some input, such as a time-varying position vector, $\vec{r}(t)$. Then varying the input t by some small amount $δt$ will change the vector by some corresponding small amount
$$δ \vec{r}(t)=\vec{r}(t+δt)-\vec{r}(t)$$
Notice that this small change in the output is itself vector-valued. The quantity 1/δt is a scalar and we know how to multiply vectors by scalars, so the ratio
$$\frac{δ \vec{r}(t)}{δt}=\frac{\vec{r}(t+δt)-\vec{r}(t)}{δt}$$
is well defined and gives an estimate of the rate of change (which in this case is the velocity).  

As in the scalar case, we can take the limit as $δt$ shrinks towards 0, and define the derivative as
$$\frac{d\vec{r}}{dt}=\\lim_{  δt\to \infty } \frac{\vec{r}(t+δt)-\vec{r}(t)}{δt}$$
This looks just like the ordinary derivative, but it is worth emphasising again that the result is a vector. This means that the derivative has both a magnitude and a direction.  

There are two quite distinct ways in which we might want to integrate with vectors. One is where we wish to integrate a vector-valued function with respect to its (scalar) input, to arrive at a vector quantity. For example, if we know the velocity of an object as a function of time, v(t), then we can determine the position of the object using
$$\vec{r}(t)=\int \vec{v}(t)\ dt$$
The other type of integral that we may want to perform gives a scalar-valued result. An example of where we might want to use this is in calculating the total distance travelled by an object. Suppose a particle travels along a path defined by the position vector $\vec{r}(t)$. Over some short time interval, the distance travelled by the particle is
$$d \ell=\sqrt{d\vec{r}\cdot d\vec{r}}$$
We can rewrite this in terms of a corresponding small change in time:
$$d \ell=\sqrt{ \frac{d\vec{r}}{dt} \cdot \frac{d\vec{r}}{dt}dt\ dt}=\sqrt{ \frac{d\vec{r}}{dt} \cdot \frac{d\vec{r}}{dt}}dt$$
Since this is scalar-valued, we can integrate as normal to find the total length along the path:
$$\ell=\int d \ell =\int\sqrt{ \frac{d\vec{r}}{dt} \cdot \frac{d\vec{r}}{dt}}dt$$
As a corollary to this, if we know the velocity as a function of time, we can immediately determine the distance travelled as
$$\ell=\int \sqrt{ \vec{v} \cdot \vec{v} }$$
[[Vector Calculus PPT.pdf]]
