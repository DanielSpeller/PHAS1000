#Mechanics #PHAS1000 #Y1 

Kinematics

Distance-time graph $s(t)$
$$v(t)=\frac{ds}{dt}$$

Speed-time graph $v(t)$
$$a(t)=\frac{dv}{dt}$$
$$\int v(t) \ dt=s(t)+c$$
Acceleration-time graph $a(t)$

$\frac{da}{dt}$ is defined as jerk
$$\int a(t) \ dt = v(t)+c$$

Deriving equations of uniform acceleration
$$a(t)=a$$
$$\frac{dv}{dt}=a$$
$$v(t)=\int a \ dt$$
$$v(t)=at+C_1$$
$$Let \ v(0) $$
$$\implies u =a(0) + C_1$$
$$C_1=u$$
$$v(t)=u+at$$


$$v(t)=u+at$$
$$\frac{ds}{dt}=v(t)$$
$$s(t)=\int v(t) \ dt$$
$$s(t)=ut+\frac{at^2}{2}+C_2$$
$$Let \ s(0) = s_0$$
$$\implies s_0=u(0)+\frac{a(0)^2}{2}+C_2$$
$$C_2=s_0$$
$$s(t)=s_0+ut+\frac{at^2}{2}$$



By eliminating u,
$$u=v-at\implies s=s_0+(v-at)t+\frac{at^2}{2}=s_0+vt-at^2+\frac{at^2}{2}=s_0+vt-\frac{at^2}{2}$$
$$s=s_0+vt-\frac{at^2}{2}$$
By eliminating t,
$$t=\frac{v-u}{a}\implies s=s_0+u(\frac{v-u}{a})+\frac{a(\frac{v-u}{a})^2}{2}$$
$$s=s_0+\frac{u(v-u)}{a}+\frac{(v-u)^2}{2a}=s_0-\frac{u^2+v^2}{2a}$$$$2as=2as_0-u^2+v^2$$
$$v^2=u^2+2as-2as_0=u^2+2a(s-s_0)$$
$$v^2=u^2+2a(s-s_0)$$
By eliminating a,
$$a=\frac{v-u}{t}\implies s=s_0 +ut+\frac{\frac{(v-u)t^2}{t}}{2}$$
$$s=s_0+ut+\frac{t(v-u)}{2}=s_0+ut+\frac{vt-ut}{2}=s_0+\frac{ut}{2}+\frac{vt}{2}$$
$$s=s_0+\frac{u+v}{2}t$$
Deriving equations of non-uniform acceleration
$$a(t)=At^2+a_0$$
$$\frac{dv}{dt}=At^2+a_0$$
$$v(t)=\int At^2+a_0 \ dt$$
$$v(t)=\frac{At^3}{3}+a_0t+C_1$$
$$Let \ v(0)=u$$
$$\implies u=\frac{A(0)^3}{3}+a_0(0)+C_1$$
$$v(t)=u+a_0t+\frac{At^3}{4}$$
$$\frac{ds}{dt}=v(t)$$
$$s(t)=\int v(t) \ dt$$
$$s(t)=ut+\frac{a_0t^2}{2}+\frac{At^4}{12}+C_2$$$$Let  \ s(0) = s_0$$
$$\implies s_0= s(t) = u(0)+\frac{a_0(0)^2}{2}+\frac{A(0)^4}{12}+C_2$$
$$C_2=s_0$$
$$s(t)=s_0+ut+\frac{a_0t^2}{2}+\frac{At^4}{12}$$


$$s(t)=A\cos(\omega t)$$
$$v(t)=\frac{ds}{dt}$$
$$Let \  \omega t=u, \frac{du}{dt}=\omega$$
$$s(t)=A\cos(u), \frac{ds}{du}=-A\sin(U)$$
$$\frac{ds}{dt}=\frac{ds}{du}\cdot\frac{du}{dt}$$
$$\frac{ds}{dt}=A\omega \cdot -\sin(\omega t)$$
$$v(t)=A\omega\cdot-\sin(\omega t)$$
$$a(t)=\frac{dv}{dt}$$
$$Let \  \omega t=u, \frac{du}{dt}=\omega$$$$v=(t)=A\omega\cdot -\sin(u), \frac{dv}{du}=A\omega\cos(U)$$$$\frac{dv}{dt}=\frac{dv}{du}\cdot\frac{du}{dt}$$
$$\frac{dv}{dt}=A\omega^2\cos(\omega t)$$
$$a(t)=A\omega^2\cos(\omega t)$$


$$s(t)=Be^{\frac{t}{\tau}}$$
$$v(t)=\frac{ds}{dt}=\frac{Bt}{\tau}e^{\frac{t}{\tau}}$$
$$a(t)=\frac{dv}{dt}=\frac{Bt^2}{\tau^2}e^{\frac{t}{\tau}}$$
[[1D Kinematics PPT.pdf]]

