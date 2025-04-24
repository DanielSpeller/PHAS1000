
#Y1 #Calclulus_and_Functions #PHAS1000 


There is little difference between one-dimensional vectors and scalars: graphically, a one-dimensional vector looks like a point on the real number line. We already know how to multiply numbers together, so we can define the product of two one-dimensional vectors to be the same as multiplying the corresponding scalar quantities.



The other special case we should consider is that of two perpendicular vectors. We can think of these as existing in two independent subspaces. As such, it makes sense to define their product as 0, since there is no sense in which these two values relate to each other. We are now ready to combine these ideas into the general definition of the scalar product or dot product. For any two vectors, $\vec{a}$ and $\vec{b}$, through a  
redefinition of coordinate system, we can always write $\vec{b}$ in terms of a component  parallel to a and a remaining part perpendicular to $\vec{a}$, 

$$\vec{b}=\vec{b_{\parallel}}+\vec{b_{\perp}}$$

The final piece of ordinary arithmetic we wish to retain is the concept of distributivity:
$$\lambda(\mu+v)=\lambda \mu+\lambda v$$
With this, we have
$$\vec{a}\cdot \vec{b}=\vec{a}\cdot(\vec{b_{\parallel}}+\vec{b_{\perp}})$$
$$=\vec{a} \cdot \vec{b_{\parallel}} $$
$$=|\vec{a}| \cdot |\vec{b_{\parallel}}| $$
Since,
$$|\vec{a}| \cdot |\vec{b_{\perp}}| =0$$
So the scalar product of two vectors is defined as the magnitude of one vector multiplied by the parallel component of the other  
vector in the direction of the first. Since we know how to find the components of a vector with trigonometry, this reduces to
$$\vec{a} \cdot \vec{b}=|\vec{a}|\times |\vec{b}|\cos(\theta)$$
where $\theta$ is the angle between the vectors

For any vector $\vec{a}$, the product of a with itself is
$$\vec{a} \cdot \vec{a}=|\vec{a}|\cdot|\vec{a}|\cos(\theta)$$
$$=|\vec{a}|^2$$
Notice this gives us a very useful identity for the magnitude of a vector 
$$|\vec{a}|\equiv\sqrt{\vec{a}\cdot \vec{a}}$$
Since perpendicular vectors have a scalar product of 0, it also follows that in Cartesian coordinates the basis vectors obey
$$\hat{i}\cdot \hat{i}=\hat{j}\cdot \hat{j}=\hat{k}\cdot \hat{k}=1$$
$$\hat{i}\cdot \hat{j}=\hat{j}\cdot \hat{k}=\hat{k}\cdot \hat{i}=0$$
The calculation of the scalar product is simplified by working in Cartesian coordinates. We have
$$\vec{a} \cdot \vec{b}=(a_{1}\hat{i}+a_{2}\hat{j}+a_{3}\hat{k})\cdot(b_{1}\hat{i}+b_{2}\hat{j}+b_{3}\hat{k})$$
$$=a_{1}b_{1}+a_{2}b_{2}+a_{3}b_{3}$$
Note that this ***only applies in Cartesian  coordinates.***  

Another very useful application of the scalar product is for finding the angle  between two vectors. Rearranging the definition, we have
$$\theta=\cos^{-1}\left(\frac{\vec{a}\cdot \vec{b}}{|\vec{a}|\times|\vec{b}|}\right)$$$$=\cos^{-1} \left(\frac{\vec{a}\cdot \vec{b}}{\sqrt{(\vec{a}\cdot \vec{a}) \cdot (\vec{b}\cdot \vec{b})}}\right)$$
Consider a line in 3D space. If we know the coordinates of any two points on the line, with position vectors $\vec{r_{1}}$ and $\vec{r_{2}}$, then we can find a general expression for any point, $\vec{r}$. The vector $\vec{v}=\vec{r_{2}}-\vec{r_{1}}$  is parallel to the line, since it’s the vector that takes us from $\vec{r_{1}}$ to $\vec{r_{2}}$: $\vec{r_{2}}=\vec{r_{1}}+\vec{v}$ . Therefore, if we choose some point on the line as a starting point, and then travel along the line by some multiple of $\vec{v}$, we can arrive at any arbitrary point along the line. Hence, we can describe the line as the set of points
$$\vec{r}=\vec{r_{1}}+\lambda \vec{v}$$
$$\vec{r}=\vec{r_{1}}+\lambda({\vec{r_{2}}}-\vec{r_{1}})$$
Recall that we defined the scalar product based on three principles:  
1. perpendicular vectors should have a product of 0,  
2. parallel vectors should have a product equal to the product of the magnitudes,  
3. the product should be distributive,  
What if we swap the first two conditions and require the product to be 0 for parallel vectors and the product of the magnitudes for perpendicular vectors? Just as before, there is only one definition consistent with these requirements: $\vec{a}\times\vec{b}=|\vec{a}|\times|\vec{b}|\sin(\theta)$. This  
type of product also comes up a lot in physics. However, it turns out that the situations in which this kind of product is useful actually require a vector-valued result – for example, in electromagnetism and 3D rotational motion. We define the vector product or cross product as
$$\vec{a}\times\vec{b}=|\vec{a}|\times|\vec{b}|\sin(\theta) \ \hat{n}$$
where $\hat{n}$ is a unit vector perpendicular to both a and b whose direction is determined by the “right-hand rule”.  
Similarly to the scalar product, we can determine the cross products of the basis vectors in Cartesian coordinates:
$$\hat{i}\times\hat{i}=\hat{j}\times\hat{j}=\hat{k}\times\hat{k}=0$$
and
$$\hat{i}\times\hat{j}=\hat{k}$$
$$\hat{i}\times\hat{k}=-\hat{j}$$
$$\hat{j}\times\hat{k}=\hat{i}$$
$$\hat{k}\times\hat{j}=-\hat{i}$$
$$\hat{k}\times\hat{i}=\hat{j}$$
$$\hat{j}\times\hat{i}=-\hat{k}$$
Notice that this product is **anti-commutative**:   $a\times b=-b\times a$

Using the above basis vector identities, we can write a general formula for the cross product in Cartesian coordinates:
$$\left(\begin{array}{r}
a_{1}\\
a_{2}\\ 
a_{3} \\
\end{array}\right) \times 
\left(\begin{array}{r}
b_{1}\\
b_{2}\\ 
b_{3} \\
\end{array}\right)
=
\left(\begin{array}{r}
a_{2}b_{3}-a_{3}b_{2}\\
a_{3}b_{1}-a_{1}b_{3}\\ 
a_{1}b_{2}-a_{2}b_{1} \\
\end{array}\right)
$$
This is less easy to remember than the expression for the dot product but notice that it has a cyclic pattern to it. It is also worth emphasising that, while the scalar product can be defined for vectors of any dimension, the cross product is only defined in 3 dimensions.

[[Scalar and Vector product.pdf]]
