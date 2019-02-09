---
title: "TNB Frame(Frenet-Serret Frame)"
date: 2019-02-02T09:38:47-05:00
draft: true
---

## Definition
Unlikely IJK frame, it is moving through the curve.  
To descirbe motion of particles travling along the curve  
T - $\vec{T}$ Unit Tangent Vector. Direction particle is heading.  
N - $\vec{N}$ Normal Vector. Direction particle is turning.  
B - $\vec{B}$ Binormal Vector. Direction of particle's twisting  

## How to find TNB
$\vec{T}$: Unit Tangent
$$\begin{align}&\vec{T}(s) = \vec{r}\prime(s) \text{ or } \vec{T}(t) = \frac{\vec{r}\prime(t)}{||\vec{r}\prime(t)||}\end{align}$$
$\vec{N}$: Unit Normal
$$\begin{align}
&\vec{N}(t) = \frac{\vec{T}\prime(t)}{||\vec{T}\prime(t)||} \newline 
&\text{Every vector with a constant length is perpendicular to it's Tangent vector} \newline
&\text{Proof: Let } \vec{v} \text{ have constant length} \newline
&\vec{v}\cdot\vec{v} = |\vec{v}|^2 = C^2 \newline
&\dfrac{d}{dt}(\vec{v}\cdot\vec{v}) = \dfrac{d}{dt}(C^2) \newline
&\vec{v}\prime\cdot\vec{v} + \vec{v}\cdot\vec{v}\prime = 2(\vec{v}\prime\cdot\vec{v}) = 0 \newline
&\text{So } \vec{T}(t) \perp \vec{T}\prime(t)
\end{align}$$
$\vec{B}$: Unit Binormal
$$\vec{B} = \vec{T} \times \vec{N}$$

## Curvature(곡률)
Curvature is Arc Length compared to Heading($\vec{T}$).  
How $\vec{T}$ is changing with respect to arc length.

### Arc length reparameterized vector function
$$
\vec{r}\prime(s) = \vec{T}(s)  
$$
$$
\kappa = \left|\left|\dfrac{d\vec{T}}{ds}\right|\right| = \left|\left|\vec{T}\prime(s)\right|\right|$$

### Original vector function
$$\begin{align}
\vec{T}\prime(t) = \dfrac{d\vec{T}}{dt} \rightarrow &\dfrac{d\vec{T}}{dt} = \dfrac{d\vec{T}}{ds}\cdot\dfrac{ds}{dt} \newline
&\dfrac{d\vec{T}}{ds} = \frac{\dfrac{d\vec{T}}{dt}}{\dfrac{ds}{dt}} \rightarrow ||\dfrac{d\vec{T}}{ds}|| = \frac{\||\dfrac{d\vec{T}}{dt}\||}{\||\dfrac{ds}{dt}\||}\tag 1 \newline
S(t) = \int \||r\prime\||\, dt \rightarrow & \dfrac{d}{dt}(S(t)) = \dfrac{d}{dt}\int \||r\prime\(t)||\, dt \newline
&\dfrac{ds}{dt} = ||r\prime(t)|| \tag 2 \newline
&\kappa = \frac{||\vec{T}\prime(t)||}{||\vec{r}\prime(t)||}
\end{align}$$

### With Polynomial
$$
\kappa = \frac{||\vec{r}\prime\times\vec{r}\prime\prime||}{||\vec{r}\prime||^3}
$$

## Torsion(곡선 비틀림)
$$
\tau = \frac{(\vec{r}\prime\times\vec{r}\prime\prime)\cdot\vec{r}\prime\prime\prime}{||\vec{r}\prime\times\vec{r}\prime\prime||^2}
$$
