---
title: "Monty Hall Problem"
date: 2020-06-05T10:26:21-04:00
---

## Monty Hall Problem
한 문 뒤에는 자동차가 있으며, 다른 두 문 뒤에는 염소가 있다.  
당신은 1번문을 고르곶 문 뒤에 무엇이 있는지 아는 사회자는 염소가 있는 2번문을 연다.  
그는 당신에게 "3번 문을 고르고 싶습니까?"라고 묻는다. 당신의 선택을 바꾸는것은 이득이 되는가?  

### Tree Diagram Solution
![Probability Tree Diagram](/monty_hall_tree.png)

### Law of Total Probability
W: 바꿔서 성공한 케이스  
$D_i$: i 번째문에 차가 있는 케이스($i = \\{1,2,4\\}$)

$$
\begin{align}
P(W) &= \frac{1}{3}\cdot P(W|D_1) + \frac{1}{3}\cdot P(W|D_2) + \frac{1}{3}\cdot P(W|D_3)\newline
&= 0 + \frac{1}{3} + \frac{1}{3}\newline
&=\frac{2}{3}\end{align}
$$

### Bayesian Theorem
$P(X|Y) = \frac{P(X \cap Y)}{P(Y)}$  
$P(X \cap Y) = P(X|Y)\cdot P(Y)$  
$P(Y \cap X) = P(Y|X)\cdot P(X)$  
$\frac{P(X|Y)P(Y)}{P(Y)} = P(X|Y) = \frac{P(Y|X)P(X)}{P(Y)}$

A: 1번문에 자동차  
B: 진행자 2번문 선택  
C: 3번문에 자동차

$$
\begin{align}
P(A|B) &= \frac{P(B|A)P(A)}{P(B)}\newline
&= \frac{\frac{1}{2}\cdot \frac{1}{3}}{\frac{1}{2}}\newline
&= \frac{1}{3}
\end{align}$$

$$
\begin{align}
P(C|B) &= \frac{P(B|C)P({C})}{P(B)}\newline
&= \frac{1\cdot \frac{1}{3}}{\frac{1}{2}}\newline
&= \frac{2}{3}
\end{align}
$$
