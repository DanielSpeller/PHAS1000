#PHAS1000 #Calclulus_and_Functions #Y1 

The Fourier Transform is a fundamental mathematical tool used to analyse functions in terms of their frequency components. It generalizes the concept of [[Fourier Series|Fourier series]] to non-periodic functions, allowing us to represent signals in the frequency domain.


A periodic function $f(x)$ with period $L$ can be expressed as a sum of sine and cosine terms:

$$
f(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} a_n \cos\left(\frac{2\pi nx}{L}\right) + b_n \sin\left(\frac{2\pi nx}{L}\right)
$$

where the coefficients are given by:

$$
a_n = \frac{2}{L} \int_{-L/2}^{L/2} f(x) \cos\left(\frac{2\pi nx}{L}\right) dx
$$

$$
b_n = \frac{2}{L} \int_{-L/2}^{L/2} f(x) \sin\left(\frac{2\pi nx}{L}\right) dx
$$

Using Euler’s formula:

$$
e^{i\theta} = \cos\theta + i\sin\theta
$$

we rewrite cosine and sine in terms of exponentials:

$$
\cos x = \frac{e^{ix} + e^{-ix}}{2}, \quad \sin x = \frac{e^{ix} - e^{-ix}}{2i}
$$

This allows us to express the Fourier series in terms of complex exponentials:

$$
f(x) = \sum_{n=-\infty}^{\infty} c_n e^{i2\pi nx/L}
$$

where the Fourier coefficients are given by:

$$
c_n = \frac{1}{L} \int_{-L/2}^{L/2} f(x) e^{-i2\pi nx/L} dx
$$

This complex form is more compact and useful for further generalization.


Now, we extend the Fourier Series to non-periodic functions. A periodic function repeats every $L$, but for a function that does not repeat, we consider the limit as $L \to \infty$.

We introduce a new variable $p = 2\pi n/L$, representing continuous frequencies. The Fourier coefficients then become a function:

$$
\tilde{f}(p) = \lim_{L\to\infty} \frac{c_n}{\delta p}
$$

This leads to the Fourier Transform:

$$
\tilde{f}(p) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} f(x) e^{-ipx} dx
$$

This equation transforms $f(x)$ from the time (or spatial) domain into the frequency domain.

The Inverse Fourier Transform recovers $f(x)$ from its frequency components:

$$
f(x) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \tilde{f}(p) e^{ipx} dp
$$

- The function $f(x)$ is decomposed into an infinite sum (integral) of complex exponentials.
- $\tilde{f}(p)$ tells us how much of each frequency $p$ is present in $f(x)$.

---

Find the Fourier Transform of:

$$
f(x) =
\begin{cases}
1, & -1 < x < 1 \\
0, & \text{otherwise}
\end{cases}
$$

Applying the definition:

$$
\tilde{f}(p) = \frac{1}{\sqrt{2\pi}} \int_{-1}^{1} e^{-ipx} dx
$$

Solving the integral:

$$
\tilde{f}(p) = \frac{1}{\sqrt{2\pi}} \left[ \frac{e^{-ipx}}{-ip} \right]_{-1}^{1}
$$

$$
= \frac{1}{\sqrt{2\pi}} \left( \frac{e^{-ip} - e^{ip}}{-ip} \right)
$$

$$
= \frac{1}{\sqrt{2\pi}} \frac{2i \sin(p)}{p}
$$

$$
= \frac{2\sin(p)}{\sqrt{2\pi} p}
$$

This result shows that the Fourier transform of a rectangular function is a sinc function, which appears frequently in signal processing.

---


The Fourier Transform simplifies differentiation. Taking the derivative in the time domain:

$$
\frac{d}{dx} f(x) \longleftrightarrow ip\tilde{f}(p)
$$

This means differentiation in the time domain corresponds to multiplication by $ip$ in the frequency domain. Similarly, for the second derivative:

$$
\frac{d^2}{dx^2} f(x) \longleftrightarrow -p^2 \tilde{f}(p)
$$

Thus, differential equations become algebraic equations in the Fourier domain, which are much easier to solve.

Consider:

$$
\frac{d^2y}{dx^2} + 2\frac{dy}{dx} - 3y = 0
$$

Taking the Fourier Transform:

$$
(-p^2 + 2ip - 3) \tilde{y}(p) = 0
$$

Solving for $\tilde{y}(p)$:

$$
\tilde{y}(p) = \frac{A}{p^2 - 2ip + 3}
$$

which can be solved by partial fractions and then inverse transformed back to obtain $y(x)$.


