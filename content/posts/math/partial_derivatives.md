---
title: "Partial Derivatives(Derivatives of Multivariable Functions)"
date: 2019-03-03T22:24:53-05:00
draft: true
---

## Derivative
$f(x,y)$ is a surface in $\mathbb{R}- 3$  

* it is the slope of surface at a point -> $\infty$ number of lines
* Find the slope of the tangent line to a surface at a point. we
  must give the tangent line a Direction
    * For now, we restrict our direction to in the 'X-Direction(Axis)' or
      in the 'y-Direction'
* To find the slope of tangent line in 'X-Direction', we must contain the tangent line in a plane parallel to teh xz-Plane
* Requires "y" to be constant

### Notation
$$\begin{align}
f(x,y) =& z \newline 
\frac{\partial f}{\partial x}, \frac{\partial z}{\partial x}, f\_{x}, z\_{x}:\ &\text{Holds 'y' constant} \newline
&\text{Slope of tangent line ot the surface at a point in x-direction} \\newline
\frac{\partial f}{\partial y}, \frac{\partial z}{\partial y}, f\_{y}, z\_{y}:\ &\text{Holds 'x' constant} \newline
&\text{Slope of tangent line of the surface at apoint in y-direction}
\end{align}$$

### Ex1
$$\begin{align}
f(x,y) &= 2x^2y^3-3x^2y+2x^2+3y^2+1 \newline
\frac{\partial f}{\partial x} &= 4xy^3 - 6xy + 4x \newline
\frac{\partial f}{\partial y} &= 6x^2y^2-3x^2+6y
\end{align}$$

### Ex2
$$\begin{align}
f(x,y) &= xe^{xy^2} \newline
f_{x} &= \frac{\partial}{\partial x}\[x\]e^{xy^2} + x\cdot\frac{\partial}{\partial x}\left[e^{xy^2}\right] \newline
&= e^{xy^2} + x\cdot e^{xy^2}\cdot\frac{\partial}{\partial x}[xy^2] \newline
&= e^{xy^2} + x\cdot e^{xy^2}\cdot y^2 \newline
&= e^{xy^2}(1+xy^2) \newline
f\_{y} &= x\cdot\frac{\partial}{\partial y}\left[e^{xy^2}\right] \newline
&= x\cdot e^{xy^2}\cdot\frac{\partial}{\partial y}\left[xy^2\right] \newline
&= x\cdot e^{xy^2}\cdot 2xy \newline
&= 2x^2ye^{xy^2}
\end{align}$$
