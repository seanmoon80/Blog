---
title: "Mathmatical proofs part 1"
date: 2019-06-07T22:10:37-04:00
draft: true
---

## Statements
True 또는 False인 선언적 문장  

* 2 is even - True  
* 17 is even - False  
* x is even - Not a statement.  

일반적으로 대문자 P,Q,R등을 사용해서 표기  

* Tautology - Always True
* Contradiction - Always False

### Conjunction
* P and Q - $P \land Q$

### Disjunction
* P or Q - $P \lor Q$

### Truth Tables
 P | Q | $P \land Q$ | $P \lor Q$   
---|---|---|---  
 T | T | T | T  
 T | F | F | T  
 F | T | F | T  
 F | F | F | F  

 ### Negation
* Opposite truth value
* ~P

### Implication (Conditional statement)
* If P, then Q  
* $P \implies Q$  

 P | Q | $P \implies Q$  
---|---|---  
 T | T | T  
 T | F | F  
 F | T | T  
 F | F | T  

* If you study, you will pass
* If you fix my computer, I will pay you $100

### Bi-Implication
* $P \iff Q - P \implies Q \text{ and } Q \implies P$  
* P if and only if Q  
* P iff Q  

 P | Q | $P \implies Q$ | $Q \implies P$ | $P \iff Q$  
---|---|---|---|---  
 T | T | T | T | T  
 T | F | F | T | F  
 F | T | T | F | F  
 F | F | T | T | T  

If $P \iff Q$ is true, P and Q are "equivalent"  

* $P \implies Q \implies R \implies P$

### Quantifier
* "For all", "For every", "For each" - $\forall$
* $\forall{x} \in \mathbb{N}$  
* "For some", "For at least one", "There exists" - $\exists$  
* $\exists{x} \in \mathbb{z}$, x is even

### Negation of quantifiers
* $\sim(\forall{x}, p(x)) \equiv \exists{x}, \sim{p(x)}$  
* $\sim(\exists{x},p(x)) \equiv \forall{x}, \sim{p(x)}$  
* $P \implies Q \equiv \sim{p} \lor Q$
* $\sim(P \implies Q) \equiv P \land \sim{Q}$

## Proving implications
### Direct Proof
1. Assume P is true  
2. Prove Q is true as consequence  

### Indirect proof (Contrapositive)
* $P \implies Q - \sim{Q} \implies \sim{P}$

1. Assume ~Q is true  
2. Show ~P is true as a consequence

### Contradiction
$R \implies C$ is true where C is false(contradiction)  
R must be false to make $R \implies C$ is true

* $\sim{R} \implies $ Contradiction  

1. Assume $P \land \sim{Q}$
2. show the leads to a contradiction

### Induction
Let P(n) be a statement that depends on n, where $n \in \mathbb{N}$  

1. P(1) is true. (Base case)  
2. Assume P(n) is true. (Inductive hypothesis)
3. Show $P(n) \implies P(n+1)$