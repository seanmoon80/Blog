---
title: "The Dot Product"
date: 2019-05-17T22:29:39-04:00
draft: true
---

$$\begin{align}
\vec a &= < a_1, a_2, a_3 >,\ \vec b = < b_1, b_2, b_3 > \newline
\vec a \cdot \vec b &= a\_1 \cdot b\_1 + a\_2 \cdot b\_2 + a\_3 \cdot b\_3
\end{align}$$

### Example 1
$$\begin{align}
\vec v &= 2\hat i - 3\hat j + \hat k,\ \vec w = -\hat i + 2\hat j - 2\hat k \newline
\vec v \cdot \vec w &= -2 - 6 - 2 = -10
\end{align}$$

### Properties
1. $\vec v \cdot \vec w = \vec w \cdot \vec v$  
2. $\vec v\cdot(\vec u + \vec w) = \vec v \cdot \vec u + \vec v \cdot \vec w$  
3. $(C\vec v)\cdot\vec w = C(\vec v \cdot \vec ) = \vec v\cdot(C\cdot\vec w)$  
4. $\vec 0\cdot \vec v = 0$  
5. $\vec v \cdot \vec v = v\_1^2 + v\_2^2 + v\_3^2 = (\sqrt{v\_1^2 + v\_2^2 + v\_3^2})^2 = ||\vec v||^2$  
6. $||\vec v|| = \sqrt{\vec v \cdot \vec v}$

### Law of Cosines
![Law of Consines](/Triangle_with_notations_2.svg)  

* $a^2 = b^2 + c^2 - 2bc\cos\alpha$  
* $b^2 = a^2 + c^2 - 2ac\cos\beta$  
* $c^2 = a^2 + b^2 - 2ab\cos\gamma$  

$$\begin{align}
||\vec v - \vec w||^2 &= ||\vec v||^2 + ||\vec w||^2 - 2||\vec v||\cdot||\vec w||\cos\theta \newline
&= (\vec v - \vec w)\cdot(\vec v - \vec w) \newline
&= \vec v \cdot \vec v - 2\vec v \cdot \vec w + \vec w + \vec w \newline
&= ||\vec v||^2 - 2\vec v \cdot \vec w + ||\vec w||^2 \newline\newline
||\vec v||^2 - 2\vec v \cdot \vec w + ||\vec w||^2 &= ||\vec v||^2 + ||\vec w||^2 - 2||\vec v||\cdot||\vec w||\cos\theta \newline
\vec v\cdot\vec w &= ||\vec v||\cdot||\vec w||\cos\theta \newline
\cos\theta &= \frac{\vec v\cdot\vec w}{||\vec v||\cdot||\vec w||} \newline
\theta &= \cos^{-1}(\frac{\vec v\cdot\vec w}{||\vec v||\cdot||\vec w||})
\end{align}$$

### Projection
![Projection Vector](/parallelprojection1.jpg)  

The Magnitude of $Proj_{\vec v}\vec u$ is called _Scalar_ or _Component_ projection $Comp\_{\vec v}\vec u$  
$$\begin{align}
\cos\theta &= \frac{Comp\_{\vec v}\vec u}{||\vec u||} \newline
Comp\_{\vec v}\vec u &= ||\vec u||\cos\theta \newline
\cos\theta &= \frac{\vec v \cdot \vec u}{||\vec v||\cdot||\vec u||} \newline
Comp\_{\vec v}\vec u &= ||\vec u||\cdot\frac{\vec v \cdot \vec u}{||\vec v||\cdot||\vec u||} = \frac{\vec v \cdot \vec u}{||\vec v||}\newline
\underbrace{Comp\_{\vec v}\vec u = ||\vec u||\cos\theta}\_{\text{If }\theta\text{ given}}&\text{ OR } \underbrace{Comp\_{\vec v}\vec u = \frac{\vec v \cdot \vec u}{||\vec v||}}\_{\theta\text{ not given}} \newline\newline
\text{Vectors } &= \text{Magnitude}\cdot\text{Direction} \newline
Proj\_{\vec v}\vec u &= Comp\_{\vec v}\vec u\cdot\underbrace{\frac{\vec v}{||\vec v||}}\_{\text{Unit vector of }\vec v} \newline
&= \frac{\vec v\cdot\vec u}{||\vec v||}\cdot\frac{\vec v}{||\vec v||} = \frac{\vec v \cdot \vec u}{||\vec v||}\cdot\frac{1}{||\vec v||}\cdot(\vec v) \newline
&= (\frac{\vec v \cdot \vec u}{||\vec v||^2})\cdot\vec v
\end{align}$$

### Example 2
$$\begin{align}
\vec a &= \hat i + 2\hat j + 3\hat k \newline
\vec b &= 2\hat i - \hat j + \hat k \newline
Proj\_{\vec a}\vec b &= (\frac{\vec a \cdot \vec b}{||\vec a||^2})\vec a \newline
&= \frac{3}{14}(\hat i + 2\hat j + 3\hat k) \newline
Proj\_{\vec b}\vec a &= \frac{3}{6}(2\hat i - \hat j + \hat k)
\end{align}$$