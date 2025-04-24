#Calclulus_and_Functions #PHAS1000 #Y1 
$$\left|\begin{array}
 {}a &b \\ c& d
\end{array}\right|=ad-bc$$
$$\left|\begin{array}
{}a&b&c \\ d&e&f \\ g&h&i
\end{array}\right|=a\left|\begin{array}
{}e&f\\h&i
\end{array}\right|-b\left|\begin{array}
{}d&f\\g&i
\end{array}\right|+c\left|\begin{array}
{}d&e\\g&h
\end{array}\right|$$
$$\det (B)\times \det(A)=\det(BA)$$
If we have matrix $A$ and $B$, and
$$BA=I$$
where $I$ is the inverse matrix, the B is the inverse matrix $A^{-1}$ if $\det(A) \neq 0$.
$$\left(\begin{array}{}
a&b\\c&d
\end{array}\right)^{-1}=\frac{\left(\begin{array}
{}d&-b\\-c&a
\end{array}\right)}{\det (A)}$$
$$\left(\begin{array}
{}a&b&c\\d&e&f\\g&h&i
\end{array}\right)^{-1}=\frac{1}{\det (A)}(\begin{array}
{}
\end{array})$$
**Gaussian reduction**
A system of linear equations of the form 
$$ax+by=c$$
$$dx-ey=f$$
can be expressed in matrices as 
$$\left(\begin{array}
{}a&b\\c&d
\end{array}\right)\left(\begin{array}
{}x\\y
\end{array}\right)=\left(\begin{array}
{}p\\q
\end{array}\right)$$
Expressed as an augmented matrix is 
$$\left(\begin{array}{cc|c} 
a&b&p \\ c&d&q
\end{array}\right)$$
[[Determinants and inverses PPT.pdf]]
