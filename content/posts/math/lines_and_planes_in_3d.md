---
title: "Lines and planes in 3d"
date: 2018-12-30T16:53:41-05:00
---

## Lines and Direction vector
선 L이 주어진 점 P1 $\(x_1, y_1, z_1)$을 지나고 방향벡터 $\vec v \<a,b,c>$와 평행시
L의 방정식 
$$
\vec L = t\cdot\vec v \\\\  
\text{Other point }P(x,y,z)\text{ on the line}\\\\   
\vec L = \vec{P\_0 P} = < x - x\_0, y - y\_0, z - z\_0 >\\\\  
\text{Direction Vector }\vec v = < a, b, c >\\\\  
\vec{P\_0 P} = t\cdot\vec v\\\\  
< x - x\_0, y - y\_0, z - z\_0 > = t\cdot< a,b,c >\\\\  
x= x\_0 + at,\ y = y\_0 + bt,\ z = z\_0 + ct \rightarrow \text{Parametric EQ of Line in 3D}\\\\  
t = \frac{x - x\_0}{a},\ t = \frac{y - y\_0}{b},\ t = \frac{z - z\_0}{t} \rightarrow \text{Symmetric EQ of Line}\\\\
$$

* $a = 0 \rightarrow x = x\_0$ Line lies in yz-plane
* Lines are parallel if their direction vectors are parallel $\vec v\_1 = t\cdot\vec v\_2$

### Example 1
$L\_1 \rightarrow x\_1 = 1 - 2t\_1,\ y\_1 = -1 - 3t\_1,\ z\_1 = -2 + t\_1$  
$L\_2 \rightarrow x\_2 = -3 + t\_2,\ y\_2 = -2 + 2t\_2, z\_2 = 3 - t\_2$  
Do $L\_1$ and $L\_2$ intersect?  
$\vec v\_1 = < -2, -3, 1>,\ \vec v\_2 = < 1, 2, -1 >$  
Intersection: $x\_1 = x\_2,\ y\_1 = y\_2,\ z\_1 = z\_2$  
$1-2t\_1 = -3 + t\_2$  
$-1 -3t\_1 = -2 + 2t\_2$  
$-2+t\_1 = 3 - t\_2$  
$t\_1 = -1, t\_2 = 6 \rightarrow -1 + 3 = -2 + 12$  
  
### How to find angle between planes as they collide:
$\cos\theta = \frac{\vec a \cdot \vec b}{||\vec a||\cdot||\vec b||} \rightarrow \cos^{-1}(\frac{\vec a \cdot \vec b}{||\vec a||\cdot||\vec b||})$

## Vector Cross Product
$\vec{v\_1} = a\_1\hat i + b\_1\hat j + c\_1\hat k$  
$\vec{v\_2} = a\_2\hat i + b\_2\hat j + c\_2\hat k$  
$\vec{v\_1} \times \vec{v\_2} = (b\_1c\_2 - c\_1b\_2)\hat i - (a\_1c\_2 - c\_1a\_2)\hat j - (a\_1b\_2 - b\_1a\_2)\hat k$  

* $\vec a \times \vec b \rightarrow $ Mutually orthogonal to $\vec a$ and $\vec b$

## Planes in R-3
How to define plane contains Point $P\_0(x\_0, y\_0, z\_0)$ and normal vecter $\vec n = < a, b, c>$  
$P\_0(x\_0, y\_0, z\_0)$ and $P(x,y,z)$ on the plane  
$\vec{P\_0 P} = < x-x\_0, y-y\_0, z-z\_0 >$  
$\vec n \cdot \vec{P\_0 P} = 0$  
$a(x - x\_0) + b(y -y\_0) + c(z-z\_0) = 0 \rightarrow $ Standard Form  
$ax + by + cz = \underbrace{ax\_0 + by\_0 + cz\_0}\_{d} \rightarrow $ General Form
