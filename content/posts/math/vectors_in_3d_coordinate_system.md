---
title: "Vectors in 3d Coordinate System"
date: 2019-05-10T21:10:47-04:00
draft: true
---

## 3D Coordinate system
* Denoted Point(x, y, z)
* Quadrant -> Octants

### Distance
$$\begin{align}
\text{Distance: } &P\_1(x\_1, y\_1, z\_1),\ P\_2(x\_2, y\_2, z\_2) \newline  
d(P\_1,P\_2) = &\sqrt{(x\_2 - x\_1)^2 + (y\_2 - y\_1)^2 + (z\_2 - z\_1)^2}
\end{align}$$

### Midpoint
$$\begin{align}
\text{Midpoint: } (\frac{x\_1 + x\_2}{2}, \frac{y\_1 + y\_2}{2}, \frac{z\_1 + z\_2}{2})
\end{align}$$

### Shapes
* Spheres - $(x - h)^2 + (y - k)^2 + (z-L)^2 = r^2$
    - Centre: (h,k,L)
    - Radius: r

### Example 1
$$\begin{align}
2x^2 + 2y^2 + 2z^2 - 6x - 4y + 2z -1 &= 0 \newline
2x^2 - 6x + 2y^2 - 4y + 2z^2 + 2z &= 1 \newline
x^2 - 3x + y^2 - 2y + z^2 + z &= \frac{1}{2} \newline
x^2 - 3x + \frac{9}{4} + y^2 - 2y + 1 + z^2 + z + \frac{1}{4} &= \frac{1}{2} + \frac{9}{4} + 1 + \frac{1}{4}\newline
(x - \frac{3}{2})^2 + (y - 1)^2 + (z + \frac{1}{2})^2 &= 4
\end{align}$$

## Vectors In R-3
### Position vector
* $\vec v = < v\_1, v\_2, v\_3 > = v\_1\hat i + v\_2\hat j + v\_3\hat k$
* $||\vec v|| = \sqrt{v\_1^2 + v\_2^2 + v\_3^2}$
* Vectors are parallel if they are _Scalar Multiples_
    - $\vec a || \vec b \text{ If } \vec a = C\cdot\vec b$

### Example 2
Show $\vec a = \hat i - 2\hat j + 5\hat k$ is $|| \vec b$ when $\vec b = <3, -6, 15>$  
$\vec b = 3\cdot\vec a$

### Example 3
$$\begin{align}
\vec a &= -\hat i + 2\hat j,\ \vec b = <2,3,-1> \newline
2\vec a - 3\vec b &= (-2 - 6)\hat i + (4 - 9)\hat j + 3\hat k \newline
&= -8\hat i - 5\hat j + 3\hat k \newline
||3\vec a|| &= || -3\hat i + 6\hat j|| \newline
&= \sqrt{9 + 36} = 3\sqrt{5}
\end{align}$$

### Example 4
$A(2,1,0),\ B(1,4,5)$ Find Position vector $\vec{AB}$  
$\vec v = <1-2,4-1,5-0> = <-1,3,5>$

### Exmaple 5
$\vec v = -\hat i + 3\hat j - \hat k$ Find _unit vector_  
$\hat u = \frac{\vec v}{||\vec v||} = \frac{-\hat i + 3\hat j - \hat k}{\sqrt{11}}$