#Complex_Number_and_Differential_Equations #PHAS1000 #Y1 
An ODE is an equation involving derivatives of an unknown function of a single variable.

The order of a differential equation is the order of the highest derivate in the equation
A linear ODE of order n is an equation in the form 
$$\frac{d^ny}{dx^n}+a_{n-1}\frac{d^{n-1}y}{dx^{n-1}}+\dots a_{n}\frac{dy}{dx}+a_{0}y=g(x)$$
An inhomogeneous linear ODE has 
$$g(x) \neq 0$$
A homogeneous linear ODE has
$$g(x)=0$$The four methods fir solving first order ODE's are
- Direct integration
- Separation of variables
$$\frac{dy}{dx}=\frac{g(x)}{h(y)}$$
- Integrating factor method
$$\frac{dy}{dx}+P(x)y=Q(x)$$
$$\frac{d[I(x)y]}{dx}=I(x)\frac{dx}{dy}+y\frac{dI(x)}{dx}=I(x)\frac{dy}{dx}+I(x)P(x)y$$
$$y\frac{dI(x)}{dx}=I(x)P(x)y$$
$$\int \frac{dI(x)}{I(x)}=\int P(x)$$
$$\ln I(x)=\int P(x)$$
$$I(x)=e^{\int P(x)}$$
$$I(x)y=\int I(x)q)Q(x)dx$$
- Homogenous equation method
$$\frac{dy}{dx}=f\left( \frac{y}{x} \right)$$
$$v=\frac{y}{x}$$
$$y=vx$$
$$\frac{dy}{dx}=v+x\frac{dv}{dx}$$
$$v+x \frac{dv}{dx}=f(v)$$
$$x\frac{dv}{dx}=f(v)-v$$
$$\int \frac{dv}{f(v)-v}=\int \frac{dx}{x}$$

