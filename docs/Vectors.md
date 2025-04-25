#Calclulus_and_Functions #Y1 #PHAS1000 
Vectors are objects that obey many of the same rules of arithmetic as ordinary numbers but which allow us to work in multiple dimensions. In particular, we can add two vectors, and multiply a vector by an ordinary real number. We can think of them as “numbers with direction”: that is, each vector has a direction and a magnitude. One way to represent vectors is as arrows: the direction of the arrow is the same as the direction of the vector, and the length of the arrow is proportional to the magnitude of the vector.  

We can add vectors graphically by connecting them “nose to tail”

![[vector_addition.excalidraw]]

We can also find graphically the result of multiplying a vector by a scalar.  Simply scale the length of the arrow by the scalar quantity but keep the direction the same.

Two vectors are parallel if they are scalar multiples of each other in this sense.  Notice that we have managed perfectly well so far talking about vectors without  introducing a coordinate system. This is because vectors are well-defined objects independently of any coordinate system. This is an important point and one that is sometimes forgotten in physics. However, for most purposes, the introduction of a coordinate system makes working with vectors much easier. The way to do this is to choose a number of vectors (equal to the dimension of the system of  
interest) and define these to be the basis vectors. Basis vectors can be chosen in any way we please as long as no two are parallel, and are usually denoted $\hat{i}$ and $\hat{j}$  etc. The vectors that we choose are known as the *basis* for the coordinate system. Any vector can then be described as a linear combination of these basis vectors.

It is worth repeating that the coordinate system we choose to work in is arbitrary. The vector is an independent object that does not require a coordinate system to exist. Depending on the situation, some coordinate systems may be more useful than others. Often, we will want to change coordinate systems to make calculations more straightforward. As long as we know the relationship  
between the basis vectors in each system, we can do this by substitution. Most often, the reason for changing coordinate systems is because it reduces one or more components to 0, simplifying further computation. For example, in the situation of a block sliding down a ramp, where we wish to model the forces acting on the block, we are free to use a coordinate system with basis vectors in the horizontal and vertical directions. However, in this system, the relevant forces will have non-zero components in both directions. Much easier is to use a coordinate system with basis vectors directed along the slope and perpendicular to it.  

[[Vectors PDF.pdf]]
