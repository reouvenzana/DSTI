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

## 4 Binomials

### 4.1 Proposition - Pascal's formula
$\displaystyle E=\{a,\dotsc ]$

The number of combinations *containing* $\displaystyle a$ is $\displaystyle C_{n-1}^{p-1}$ (since $\displaystyle a$ is always selected).

The number of combinations *not containing* $\displaystyle a$ is $\displaystyle C_{n-1}^{p}$ (since we remove $\displaystyle a$ from $\displaystyle n$).

Then, the number of combinations containing $\displaystyle a$ added to the number of combinations not containing $\displaystyle a$ is equal to the total number of combinations.

$\displaystyle C_{n}^{p} =C_{n-1}^{p-1} +C_{n-1}^{p}$

### 4.2 Proposition - Binomial's formula $\displaystyle ( +)$
$\displaystyle ( x+a_{1})( x+a_{2}) \dotsc ( x+a_{n})$
$\displaystyle =x^{n} +\sigma _{1} x^{n-1} +\sigma _{2} x^{n-2} +\dotsc +\sigma _{p} x^{n-p} +\dotsc +\sigma _{n}$

With:
$\displaystyle \sigma _{1} =a_{1} +\dotsc +a_{n}$

$\displaystyle \sigma _{2} =\sum _{i\neq j} a_{i} a_{j} =C_{n}^{2}$

$\displaystyle \sigma _{p} =\sum a_{i} \dotsc a_{p} =C_{n}^{p}$

$\displaystyle \sigma _{n} =\sum a_{1} \dotsc a_{n} =C_{n}^{n} =1$

### 4.3 Proposition - Binomial's formula $\displaystyle ( -)$
$\displaystyle ( x-a_{1})( x-a_{2}) \dotsc ( x-a_{n}) \ =x^{n} -\sigma _{1} x^{n-1} +\sigma _{2} x^{n-2} +\dotsc +( -1)^{p} \sigma _{p} x^{n-p} +( -1)^{n} \sigma _{n}$

### 4.4 Proposition - $\displaystyle a_{1} =a_{2} =\dotsc =a_{n}$
$\displaystyle ( x+a_{1})( x+a_{2}) \dotsc ( x+a_{n}) =( x+a)^{n}$

Then:
$\displaystyle ( x+a)^{n} =x^{n} +na^{1} x^{n-1} +C_{n}^{2} a^{2} x^{n-2} +\dotsc +C_{n}^{p} a^{p} x^{n-p} +a^{n}$

> [!example] Example
> $\displaystyle n=3$<br>
> $\displaystyle ( x+a)^{3} =x^{3} +3ax^{2} +2a^{2} x+a^{3}$

### 4.5 Proposition - $\displaystyle x=a=1$
$\displaystyle ( 1+1)^{n} =2^{n} =\sum _{p=0}^{n} C_{n}^{p}$

### 4.6 Proposition - sum of combination of odds and even
$\displaystyle \sum _{p=\text{odd}} C_{n}^{p} =\sum _{p=\text{even}} C_{n}^{p} =2^{n-1}$

### 4.7 Proposition - square of a polynomial
$\displaystyle \underbrace{( a+b+\dotsc +l)^{2}}_{n^{2}\text{ terms}} =\underbrace{\sum a^{2}}_{n\text{ terms}} +2\underbrace{\sum ab}_{C_{n}^{2}\text{ terms}} +\dotsc$

### 4.8 Proposition - cube of a polynomial
$\displaystyle \underbrace{( a+b+\dotsc +l)^{3}}_{n^{3}\text{ terms}} =\underbrace{\sum a^{2}}_{n\text{ terms}} +3\underbrace{\sum a^{2} b}_{A_{n}^{2}\text{ terms}} +6\underbrace{\sum abc}_{C_{n}^{3}\text{ terms}} + \dotsc$

