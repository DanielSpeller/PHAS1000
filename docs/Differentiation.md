#Calclulus_and_Functions #PHAS1000 #Y1 
The following derivation of the concept of differentiation is probably familiar. However, it is worth revisiting, as we will generalise this idea later to new contexts. Often we want to know the rate at which a function’s output varies with respect to its input. For sufficiently small $δx$, a good approximation to this rate of change is $\frac{\delta f(x_{0})}{\delta x}$. Note that we normalise the rate by scaling down by $δx$. Without taking this ratio, the “rate of change” would depend on the particular δx we choose. Choosing a large $δx$ is not going to give us a very good estimate of the rate  
of change. This is because the rate of change can itself vary at different inputs. For example, if the function is increasing at $x_{0}$ but then starts to decrease for larger $x$, a small $δx$ can give a positive rate of change, while a large $δx$ may give a negative rate of change. Our estimate of the rate of change improves as we make $δx$ smaller. So if we allow $δx$ to decrease and become arbitrarily close to 0, we will hone in on the exact value of the rate of change. We define the derivative of $f$ at $x_{0}$ as:

$$\frac{df(x_{0})}{dx}=\lim_{ \delta x \to 0 } \frac{\delta f(x_{0})}{\delta x}=\lim_{ \delta x \to 0 } \frac{f(x_{0}+\delta x)-f(x_{0})}{\delta x}$$
This process of taking the limit of the ratio between the changes in output and input values of the function is differentiation. It is worth remembering that this is the definition of differentiation and that everything else related to the concept follows from here. Later, when we generalise differentiation to less familiar contexts, this is the key concept that we wish to keep. Note that we have, so far, defined the derivative of a function at a point. Since the point $x_{0}$ was arbitrary, we could equally choose a different fixed point, $x_{1}$ and find the derivative of the function at this new point: $\frac{df(x_{1})}{dx}$. In fact, since we can choose any base point, the collection of such derivatives is itself a  
function: 
$$f ^{′}(x) ≡ \frac{df(x)}{dx}$$
$$f(x)=x^n$$
$$\frac{df}{dx}=\lim_{ \delta x \to 0 }\frac{(x+\delta x)^n-x^n}{\delta x} $$
$$\frac{df}{dx}=\lim_{ \delta x \to 0 }\frac{\sum_{k=0}^n \left(\begin{array} (n \\ k
\end{array}\right)}{\delta x}$$
<h4>Chain Rule</h4>
$$u=f(x)$$
$$y=g(u)$$
$$f:A \to B$$
$$g: B \to C$$
$$h=g\circ f : A\to C $$
$$y=h(x)=g(f(x))$$
$$\frac{dy}{dx}=\frac{dy}{du} \frac{du}{dx}$$
$$h'(a)=g'(f(a))\cdot f'(a)$$

[[Differentiation PPT.pdf]]
