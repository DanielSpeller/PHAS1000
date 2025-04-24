#Calclulus_and_Functions #PHAS1000 #Y1 
A function, $f$ , is a map between two sets of objects: the **domain**, $A$, and the **codomain**, $B$. For each element $x$ of $A$, there is a unique element $f (x)$ in $B$.  We denote the relationship between the function and the sets by $f : A → B$, and we can show the action of $f$ on a particular element as $f : x \mapsto f (x)$. The sets $A$  and $B$ are part of the definition of the function. Although every element in the domain has associated with it an element of the codomain, the converse is not necessarily true: there can be elements of the codomain to which no element in $A$ are mapped by $f$ . The set of elements that are mapped to is called the range of the function. The value input to a function is often called the argument, while value is generally reserved for the output.  


The definition of a function is extremely broad and allows very abstract functions. However, the most useful functions tend to be those that map from some mathematical structure to another. The most commonly used functions map from the real numbers to the real numbers. These are the functions that we are interested in here.

<h3>Graphs of Functions</h3>
We can use a two-dimensional Cartesian coordinate system, $x, y$ , to depict a function as a graph. Specifically, we can produce a curve which is the locus of points of the form $(x, f (x))$ for $x ∈ A$. While software can graph any function easily, this does not always help us to understand a function. The best way to understand a function is to sketch its graph manually. To do this, there are a set of key features that we are typically interested in, including zeros or roots, intercept, range, stationary points, inflection points, and asymptotes.

<h4>Intercept</h4>  
The intercept is the simplest of these key features to determine. It is simply the value of the function evaluated at 0. In terms of the graph of the function, this is its value where it intercepts the y axis. As long as the domain contains 0, there will always be exactly one intercept

<h4>Roots</h4>  
The roots of a function are the values of the input $x$ for which the output is 0. In terms of the graph, these are any points at which the graph intersects the $x$ axis. Depending on the function, there could be any number of roots from 0 to infinitely many. For example, $f (x) = x^2 + 2$ has no roots, $f (x) = x + 1$has one at $x = −1$, $f (x) = x^2 − 4$ has two $x = ±2$, and $f (x) = sin(x)$ has a root at every integer multiple of $π$. Finding the roots of a function involves solving the equation $f (x) = 0$ and the method for doing this will typically depend on the function.  

<h4>Stationary Points </h4>  
The stationary points of a function are those points for which $f ^{′}(x) = 0$. This is where the gradient of the graph vanishes. For a simple function with only one input, there are only three types of stationary point: maxima and minima (collectively extrema), and saddle points. To find any of these, we must first  
differentiate the function and then solve $f^{\prime}(x) = 0$. As with roots, the method of solution of this equation can vary greatly between functions. Once we have found the location of any stationary points, we must also determine their nature. For this we use the second derivative.

<h4>Second Derivatives </h4>
Since the derivative gives the slope of a function (or its graph), a positive derivative means the function is increasing, and a negative derivative means the function is decreasing. In between, when the derivative is exactly 0, the function is neither increasing nor decreasing, which is why we find the maximum or minimum value here. Similarly, the second derivative is the rate of change of the  
derivative. So a positive second derivative means the first derivative (slope) is increasing. This in turn means that the graph at this point is curving upwards. Similarly, a negative second derivative means that the first derivative is decreasing and the graph curves down. In between, we have a point of inflection, at which $f ^{′′}(x) = 0$ and there is no curvature. The graph in this region is locally or momentarily linear. The second derivative also allows us to determine the nature of stationary points. If $f ^{\prime\prime}(x) < 0$ at a stationary point, the slope is 0 but the graph curves down, so we must have a maximum. Likewise, if $f ^{\prime\prime}(x) > 0$ at a stationary point, then it is a minimum. While this is a useful test, in some  
situations, we find $f ^{\prime\prime}(x) = 0$ and we must find an alternative way to determine the nature of the stationary point. For example, if all stationary points are known, we can use the relative values of $f$ at the neighbouring stationary points on either side to determine the nature of the middle one. A saddle point is simultaneously a stationary point and a point of inflection. The name “saddle point” does not make much sense in this context, but will become clearer when we consider functions of more than one variable

<h4>Asymptotes and values at infinity</h4>  
A vertical asymptote is a value that is not contained in the domain of a function, where the value of the function nearby tends towards $±∞$ as the argument tends to the asymptote. Such values are sometimes also referred to as singular points or poles. For example, the function $f : \mathbb{R}\backslash{0} → \mathbb{R}, f (x) = 1/x$ is not defined at $x = 0$ but the value of the function near $x = 0$ grows without limit. Notice that the value $f$ tends to need not be the same on each side of the asymptote: in this  
case $\lim_{x→0+} = ∞$, while $\lim_{x→0-} = -∞$. However, there are also functions for which the two limits are the same, for example $f (x) = \frac{1}{x^2}$. 

We also often want to know about the value of a function as $x → ±∞$. Some functions grow without limit for large $x$, but others may gradually tend towards a finite value. In this case, they are said to have a horizontal asymptote. The way to test for this is to manipulate the expression for the function until its  behaviour at $±∞$ is clear. For example, the function
$$f(x)=\frac{1+2x}{x-4}$$
tends to 2 as $x \to \infty$. To see this, divide the numerator and denominator by $x$ to get
$$f(x)=\frac{\frac{1}{x}+2}{x-\frac{4}{x}}$$
For large values of $x$, this is approximately
$$f(x)\approx \frac{0+2}{1-0}=2$$
<h4>Range</h4>
In order to find the range of a function, we must consider all stationary points and vertical asymptotes, and the behaviour of the function at $±∞$. Let’s consider the maximum value of the function (everything we say can be reversed for the minimum value). If the function has vertical asymptotes at which its value tends to $+∞$ from either side, or if the value of the function at $x → ±∞$ tends towards $+∞$, then there is no maximum value of the function: the function is  unbounded from above. If neither of these points is true, then the global maximum value of the functions is the largest of the local maxima determined by the stationary points.

<h4>Function Composition</h4>
Gives functions $f:A \to B$ and $g:B \to C$, we can define the composite function $g \circ f:A \to C$ as
$$(g \circ f)(x)=g(f(x)) \forall x \in A$$
That is, if $f$ maps $x$ to $y$ and $g$ maps $y$ to $z$, then $g \circ f$ maps $x$ directly to $z$
<h4>Inverse functions</h4>
One particularly important application of function composition is in defining  
the inverse function. The inverse of a function f is only defined if f satisfies  
two properties:
- for every element, $b$, of $B$, there is an element, $a$, of $A$ such that $f(a)=b$
- for any two distinct elements, $x$ and $y$, of $A$, $f(x) \neq f(y)$
In this case we can define the inverse function $f^{-1}:B \to A$ such that $f^{-1} \circ f =I$, where $I:A \to A$ is the identity function $I(x)=x \forall x$ 

<h4>Circular functions</h4>
The regular trigonometric functions are defined in terms of a unit circle, $x^2 + y^2 = 1$. For this reason, they are also sometimes known as the circular functions. By definition, $\sin(θ)$ is the height of a vertical line from the $x$ axis to the circle that subtends an angle $θ$. The cosine is the horizontal distance of this line from the origin. The other trigonometric functions can also be defined in terms of various projections on this circle, but it is much easier to define them in terms of these first two:
$$\tan x=\frac{\sin x}{\cos x}$$
$$\cot x=\frac{\cos x}{\sin x}$$
$$\sec x=\frac{1}{\cos x}$$
$$\csc x=\frac{1}{\sin x}$$
as well as the useful identities:
$$\sin^2x+\cos^2x=1$$
$$\tan^2x+1=\sec^2x$$
$$1+\cot^2x=\csc^2x$$
<h4>Hyperbolic Functions</h4>
Instead of the unit circle, let’s now use the unit hyperbola, $x^2 − y^2 = 1$, to define a similar set of trigonometric functions. Since “angle” does not have any obvious meaning here, we will define these hyperbolic functions in terms of area,
$$\sinh x=\frac{e^x-e^{-x}}{2}$$
$$\cosh x=\frac{e^x+e^{-x}}{2}$$


[[Functions PPT1.pdf]]
[[Functions PPT2.pdf]]
