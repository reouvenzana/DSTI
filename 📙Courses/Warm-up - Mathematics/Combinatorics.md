# Combinatorics

## 1 Permutations

### 1.1 Definition - permutations

A **permutation** is a finite set totally *ordered*. We define a bijection between a set $\displaystyle E$ of $n$ ordered elements.

### 1.2 Proposition - number of permutations
$\displaystyle E=\{a_{1} ,a_{2} ,\dotsc ,a_{n}\}$ 
The number of permutation is $\displaystyle n!$

Proof:
$\displaystyle a_{1}$ has $\displaystyle n$ possibilities
$\displaystyle a_{2}$ has $\displaystyle n-1$ possibilities
$\displaystyle \dotsc$
$\displaystyle a_{n}$ has $\displaystyle 1$ possibility
So: $\displaystyle n( n-1)( n-2) \dotsc 1=n!$

## 2 Arrangements

### 2.1 Definition - arrangement
A **combination** is an *ordered* subset of $\displaystyle p$ elements among $\displaystyle n$.

Two arrangements differ either by the nature or their elements by the order of their elements.

### 2.2 Proposition - number of arrangements
The number of arrangement $\displaystyle A$ of $\displaystyle p$ elements among $\displaystyle n$ , with $\displaystyle p\leqslant n$ is:
 $\displaystyle A_{n}^{p} =\frac{n!}{( n-p) !}$

By convention, $\displaystyle A_{n}^{0} =1$.

#### 2.2.1 Proof
At first, there are $\displaystyle n$ possibilites, then $\displaystyle n-1$, and, eventually, $\displaystyle n-p+1$ possibilities.
$\displaystyle A_{n}^{p} =n( n-1)( n-2) \dotsc ( n-p+1)$

The $\displaystyle +1$ is necessary to make sure we don't divide by $\displaystyle 0$.

Then, $\displaystyle A_{n}^{p}$ can be written in another way:

$\displaystyle A_{n}^{p} =\frac{n( n-1) \dotsc ( n-p+1)\textcolor[rgb]{0.82,0.01,0.11}{(}\textcolor[rgb]{0.82,0.01,0.11}{n-p}\textcolor[rgb]{0.82,0.01,0.11}{)}\textcolor[rgb]{0.82,0.01,0.11}{(}\textcolor[rgb]{0.82,0.01,0.11}{n-p-1}\textcolor[rgb]{0.82,0.01,0.11}{)}\textcolor[rgb]{0.82,0.01,0.11}{\dotsc 1}}{\textcolor[rgb]{0.82,0.01,0.11}{(}\textcolor[rgb]{0.82,0.01,0.11}{n-p}\textcolor[rgb]{0.82,0.01,0.11}{)}\textcolor[rgb]{0.82,0.01,0.11}{(}\textcolor[rgb]{0.82,0.01,0.11}{n-p-1}\textcolor[rgb]{0.82,0.01,0.11}{)}\textcolor[rgb]{0.82,0.01,0.11}{\dotsc 1}}$ 
<br>
$\displaystyle A_{n}^{p} =\frac{n!}{( n-p) !}$

## 3 Combinations

### 3.1 Definition - combination
A **combination** is a* non-ordered* subset of $\displaystyle p$ elements among $\displaystyle n$. 

Two combinations differ only by the nature of their elements, not by the order of the elements.

### 3.2 Proposition - number of combinations
$\displaystyle C_{n}^{p} =\frac{A_{n}^{p}}{p!} =\frac{n!}{p!( n-p) !}$

### 3.3 Proposition - combination of zero element

$\displaystyle C_{n}^{0} =\frac{A_{n}^{0}}{0!} =\frac{1}{1} =1$

### 3.4 Proposition - combination of one element

$\displaystyle C_{n}^{1} =\frac{n!}{1!( n-1) !} =\frac{n( n-1)( n-2) \dotsc \times 1}{( n-1)( n-2) \dotsc \times 1} =n$

### 3.5 Proposition - combination of two elements

$\displaystyle C_{n}^{2} =\frac{n!}{2!( n-2) !} =\frac{n( n-1)( n-2) \dotsc \times 1}{2( n-2) \dotsc \times 1} =\frac{n( n-1)}{2}$

### 3.6 Proposition - combination of $n-p$

$\displaystyle C_{n}^{n-p} =C_{n}^{p}$

#### 3.6.1 Proof

$\displaystyle C_{n}^{n-p} =\frac{n!}{( n-p) !( n-( n-p)) !} =\frac{n!}{p!( n-p) !}$

### 3.7 Propositon - combination of $n$ elements
$\displaystyle C_{n}^{n} =1$

#### 3.7.1 Proof
We use [[Combinatorics#3.6 Proposition - combination of $n-p$]] and [[Combinatorics#3.3 Proposition - combination of zero element]]

$\displaystyle p=n$, so

$\displaystyle C_{n}^{n} =C_{n}^{n-n} =C_{n}^{0} =1$

## 4 Pascal's formula

