---
title: "Random variables"
date: 2020-05-01T22:15:21-04:00
---

## Bernoulli Random Variables
Bernoulli with parametr $p \in [0, 1]$  
$X = 
\begin{cases}
1, p \newline  
0, 1 - p
\end{cases}
$  
* Either Success or failure  
* Either Heads or Tails  
* Idicator r.v. of an event A: $I\_A = 1$ iff A occurs  
* $P\_{I\_A}(1) = P(I_A = 1) = P(A)$

## Discret uniform random variable
Parameters $a, b$  
* Parameters: integers <span style="color:red">**$a, b; a \le b$**</span>  
* Experiment: $a, a + 1,...,b$ randomly pick one; all equally likely  
* Sample space: ${a,a+1,...,b}$ ($b-a+1$ Possible values)  
* Random variable $X: X(w) = w$
* Special case: $a = b$ (constant/deterministci r.v)

## Binomial random variable
Parameters: positive integer $n; p \in [0, 1]$  
* Experiment: $n$ independent tosses of a coin with $P(Heads) = p$  
* Sample space: Set of sequences of H and T, of length $n$  
* Random variable $X$: number of Heads observed  
* Model of: number of successes in a given number of independent trials  
* Binomila Formula: <span style="color:red">**$pX(k) = \binom{n}{k}p^k(1-p)^{n-k}, \text{for }k = 0,1,...,n$**</span>

## Geometric random variable
Parameter $p: 0 \lt p \le 1$  
* Experiment: infinitely many independent tosses of a coin; $P(Heads) = p$  
* Sample space: Set of infinite sequences of H and T; $\\{HTTTT...\\}$  
* Random variable X: number of tosses until the first Heads  
* Model of: waiting times; number of trials until a success  
* First Head observed in the $k$ trial:  
<span style="color:red">**$pX(k) = p(X = k) = p(\underbrace{TTT...T}_{k-1}H) = (1-p)^{k-1}p,$ $k = 1,2,3...$**</span>
