---
title: "Constrained Optimization with LaGrange Multipliers"
date: 2019-04-18T13:12:26-04:00
draft: true
---

## Example 1
$$\begin{align}
f(x,y) = xy,\ \text{constraint of } 2x+3y = 6 \newline
\nabla f(x,y) = y\hat i + x \hat j,\ \nabla g(x,y) = 2\hat i + 3\hat j \newline
y\hat i + x\hat j = 2\lambda\hat i + 3\lambda\hat j \newline
y = 2\lambda,\ x = 3\lambda \newline
2x + 3y = 6 \rightarrow 6\lambda + 6\lambda = 6 \newline
\lambda = \frac{1}{2},\ x = \frac{3}{2},\ y = 1 \newline
f(\frac{3}{2}, 1) = \frac{3}{2}
\end{align}$$

## Example 2
$$\begin{align}
f(x,y,z) = x+2y-2z,\ x^2+2y^2+4z^2=1 \newline
\nabla f(x,y,z) = \hat i + 2\hat j - 2\hat k = 2x\lambda\hat i + 4y\lambda\hat j + 8z\lambda\hat k \newline
x = \frac{1}{2\lambda},\ y = \frac{1}{2\lambda},\ z = \frac{-1}{4\lambda} \newline
x^2+2y^2+4z^2 = 1 \rightarrow (\frac{1}{2\lambda})^2 + 2(\frac{1}{2\lambda})^2 + 4(\frac{-1}{4\lambda})^2 = 1 \newline
\frac{1}{4\lambda^2} + \frac{1}{2\lambda^2} - \frac{1}{4\lambda^2} = 1 \newline
1 + 2 + 1 = 4\lambda^2 \rightarrow \lambda = 1, -1
\lambda = 1 \rightarrow x = \frac{1}{2},\ y = \frac{1}{2},\ z = -\frac{1}{4} \newline
\lambda = -1 \rightarrow x = -\frac{1}{2},\ y = -\frac{1}{2},\ z = \frac{1}{4} \newline
f(\frac{1}{2}, \frac{1}{2}, -\frac{1}{4}) = 2 \newline
f(-\frac{1}{2}, -\frac{1}{2}, \frac{1}{4}) = -2 \newline
Max = 2,\ Min = -2
\end{align}$$