---
title: "Varieties of solutions of linear systems and the determinant"
date: 2019-07-06T10:06:16-04:00
draft: true
---

## System
* Inconsistent - $(0\ 0\ 0\ ..\ 0\ |\ a)\ a \ne 0$ in REF or RREF
* Infinitely many solutions - $(0\ 0\ 0\ ..\ 0\ |\ 0)$ in REF or RREF

### Thearem
Let $A\vec x = \vec b$ be any $m \times n$ system of linear equations, $m, n \in \mathbb{Z}$
Then there are only three possible situation for the solution:

1. The system will have No solution!
2. The system will have a unique solution
3. The system will have infinite number of solutions

### Proof
Augment the system to get $(A|\vec b)$ and find its REF or RREF  
we have two cases:

1. The system is inconsistent
2. The system is consistent
    * Number of pivots = number of columns of A - Unique Solution
    * Number of pivots < number of Columns of A - Infinitely many solutions

### Rank
The rank of a matrix A is the Number of non-zero rows in its REF or RREF  
This is equal to the number of pivots rank(A)  

$A\vec x = \vec b$  
$B = (A|\vec b)$ where A is $m \times n$  

* rank(B) = rank(A) - Unique or infinite
* rank(B) < rank(A) - Impossible
* rank(B) > rank(A) - Inconsistent

### Homogeneous Systems
The system $A\vec x = \vec b$ is called homogenous if  $\vec b = \vec 0$  
Notation - $A\vec x = \vec 0$

* Homogeneous systems are ALWAYS consistent.
* They have either exactly one solution($\vec x = \vec 0$) or infinitely many
* $\vec x = \vec 0$ is called the trivial solution

## The Determinant
The Area of $A = \begin{pmatrix}a & b\\\\ c & d\end{pmatrix}$ is $(ad - bc)$  
Determinant gave the signed area of the parallelogram formed by the row vectors  
Volume of parallelopiped $ = |\vec a\cdot(\vec b \times \vec c)|$
Notation - $|A| or \det A$  

### Minor
Let A be an $n \times n$ matrix,  
The i, j<sup>th</sup> minor of A, denoted $M_{ij}$  
is the determinant of the matrix obtained by eleminating the i<sup>th</sup> row a j<sup>th</sup> column of A

$A = \begin{pmatrix}a\_{11} & a\_{12} & a\_{13}\\\\a\_{21} & a\_{22} & a\_{23}\\\\a\_{31} & a\_{32} & a\_{33}\end{pmatrix}$ $M_{23} = \begin{vmatrix}a\_{11} & a\_{12}\\\\a\_{31} & a\_{32}\end{vmatrix}$

### Cofactor
The i,j<sup>th</sup> cofactor of A, denoted C<sub>ij</sub> is given by  
$C\_{ij} = (-1)^{i+j}M\_{ij}$  
$C_{23} = -\begin{vmatrix}a\_{11} & a\_{12}\\\\a\_{31} & a\_{32}\end{vmatrix}$

### General Determinant
Let $A\_{n \times n}$ be a matrix
$\det(A) = a\_{i1}C\_{i1} + a\_{i2}C\_{i2} + ... + a\_{in}C\_{in}$ for any row i in A $\sum\_{k = 1}^n a\_{ik}C\_{ik}$
$\det(A) = a\_{1j}C\_{1j} + a\_{2j}C\_{2j} + .. + a\_{nj}C\_{nj}$ for any column j in A $\sum\_{k=1}^n a\_{kj}C\_{kj}$

### Example
$A = \begin{pmatrix}1 & 0 & 0 & -1\\\\3 & 1 & 2 & 2\\\\1&0&-2&1\\\\2&0&0&1\end{pmatrix}$

1. Choose any row or any column.
2. find the signs for the cofactors in this row or column.
3. Follow the formula  

$\det A = -0\cdot\begin{vmatrix}3&2&2\\\\1&-2&2\\\\2&0&1\end{vmatrix} + 1\cdot\begin{vmatrix}1&0&-1\\\\1&-2&1\\\\2&0&1\end{vmatrix}...\\\\
= 1(-2\cdot\begin{vmatrix}1&-1\\\\2&1\end{vmatrix})$