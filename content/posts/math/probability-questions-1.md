---
title: "Probability Questions 1"
date: 2020-05-08T19:18:57-04:00
draft: true
---

## Question 1  
나는 현재 포커 토너먼트에 진출 해 있습니다. 다음 단계로 진출 하기 위해 서는 이미 정해진 상대 A,B,C와 연속으로 반드시 게임을 해야 합니다. 나는 두 명에게 연속으로 승리하면 다음 토너먼트로 진출 할 수 있습니다.  
* 개별 게임은 전부 독립사건으로 가정  
* 나는 상대와의 승률 데이터를 가지고 있는데 각각 A를 상대로 승률 0.8 B를 상대로 0.5 C를 상대로 0.1 과 같습니다.  
* 포커 게임을 할 상대와의 매치 순서는 내가 임의로 정 할 수 있다.  
위의 조건에서 내가 2연승을 하고 다음단계로 진출 하기 위해 A,B,C와의 매치 순서를 어떻게 매열 하는게 가장 높은 승률을 보장 받을 까요?  

Experiment: Play poker game with A,B and C in any order  
  
Event: More than 2 consecutive wins  
  
Given Probability: $P(A) = 0.8, P(A^c) = 0.2, P(B) = 0.5, P(B^c) = 0.5, P(C) = 0.1, P(C^c) = 0.9$  
  
Sample Space: $\\{ABC, ABC^c, AB^cC, AB^cC^c, A^cBC, A^cBC^c, A^cB^cC, A^cB^cC^c,..., C^cA^cB^c\\}$  
  
More than 2 consecutive wins: $\\{ABC, ACB, BAC, BCA, CAB, CBA, ABC^c, BAC^c...,C^AB\\}$  
  
$\\{ABC, ACB, BAC, CAB\\}$ 의 확률은 동일(독립사건)  
  
$MAX({ABC, ABC^c, ACB^c, BCA^c}) = MAX({0.04, 0.36, 0.04, 0.01}) = ABC^c$  
  
Answer: ${ABC^c, BAC^c, C^cAB, C^cBA}$  

## Question 2
n 명의 참관인, 부정선거목격시 폭로할 확률 $1/n$ 참관인이 한없이 늘어날때 적어도 한명이 고발할 확률이 수렴하는 값  

Probability Given: $P({R}) = \frac{1}{n}, P(R^c) = 1 - \frac{1}{n}$  
  
Event: $P(\underbrace{R^cR^c...}_{n-1}R) = (1-\frac{1}{n})^{n-1}\frac{1}{n}$  
  
$\lim\limits\_{n\to\infty}(1-\frac{1}{n})^{n-1}\frac{1}{n} = 0$
