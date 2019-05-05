---
title: "An Introduction to Vectors"
date: 2019-05-03T21:29:11-04:00
draft: true
---

# Vectors
* Vectors have both a _Speed (Magnitude)_ and a _Direction_  
* Vector from point A to point B $\rightarrow \vec v = \vec{AB}$
* Vectors can multifly by Constants(Scalars)  
    * Length of vector $\rightarrow 3\vec v$  
    * Reverse Direction of vector $\rightarrow -2\vec v$  
    * $\vec v \parallel T\vec v \rightarrow T$ is some scalar

## Adding & Substracting Vectors
* $\vec v + \vec w$
* $\vec v - \vec w = \vec v + (-\vec w)$

## Position Vector
* An initial point at the _Origin_(0,0)
* A terminal point at P(v1, v2)
* Denoted $\left\<V\_1, V\_2\right\>$

### Vector to Position Vector
$$\begin{align}
P_1(1,2),\ P_2(6,4)  \newline
\vec v = \vec{P\_1 P\_2} = \left\< x\_2 - x\_1, y\_2 - y\_1\right\> = \left\<5, 2\right\>  \newline
\end{align}$$

### Slope of vector
$$
\frac{y_2 - y_1}{x_2 - x_1}
$$

### Length(Magnitude)
$$
||\vec v|| = \sqrt{(v\_1)^2 + (v\_2)^2}
$$

### Equality of vectors
$$
\text{Slope of }\vec v = \text{Slope of }\vec w  \\\\  
||\vec v|| = ||\vec w||
$$

### Example 1
$$\begin{align}
\vec a &= \left\<-1, 2\right\>,\ \vec b = \left\<3,1\right\>  \newline
2\vec a &= \left\<-2, 4\right\> \newline
\vec a + \vec b &= \left\<2, 3\right\> \newline
\vec a - \vec b &= \left\<-4, 1\right\> \newline
||2\vec a + \vec b|| &= \sqrt{1^2 + 5^2} = \sqrt{26}
\end{align}$$

## Unit Vector
* A vector with _length 1_  
* $\hat u = \frac{\vec v}{||\vec v||} \rightarrow \vec v = ||\vec v||\cdot\hat u$  
* A unit vector in _opposite direction_ $\hat u = \frac{-\vec v}{||\vec v||}$

## Standard Basis Vector
* $\hat i = \left\<1,0\right\>$ (X-Direction Unit Vector)  
* $\hat j = \left\<0,1\right\>$ (Y-Direction Unit Vector)  
* $\vec v = \left\<V\_1, V\_2\right\> = V\_1\hat i + V\_2\hat j$

### Example 2
$$\begin{align}
\vec a = -3\hat i + 4\hat j,\ \vec b = \hat i + 2\hat j  \newline
\text{Find }\vec v\text{ where } ||\vec v|| = 3\text{ and } \vec v || 2\vec a - 3\vec b  \newline
2\vec a - 3\vec b = -6\hat i + 8\hat j - (3\hat i + 6\hat j) = -9\hat i + 2\hat j \newline
\hat u = \frac{-9\hat i + 2\hat j}{\sqrt{85}} = \frac{\sqrt{85}}{85}(-9\hat i + 2\hat j) \newline
\vec v = ||\vec v||\cdot\hat u = 3\cdot\frac{\sqrt{85}}{85}(-9\hat i + 2\hat j)
\end{align}$$

## Unit Vector and Trigonometry
* $\hat u = \cos\theta\hat i + \sin\theta\hat j$

### Example 3
Find $\vec v$ such that $\vec v$ has a length of '9'  
and $\vec v$ makes  an angle of $\frac{\pi}{6}$ with X-Axis
$$\begin{align}
\hat u &= \cos{\frac{\pi}{6}}\hat i + \sin{\frac{\pi}{6}}\hat j \newline  
&= \frac{\sqrt 3}{2}\hat i + \frac{1}{2}\hat j \newline  
\vec v &= 9\cdot(\frac{\sqrt 3}{2}\hat i + \frac{1}{2}\hat j)
\end{align}$$