# Sets

## 1 Definition - inclusion
$\displaystyle A\ \in \ E$ means that $\displaystyle \forall \ x\ \in \ A,\ x\ \in \ E$.

## 2 Definition - strict inclusion
$\displaystyle A$ is strictly included in $\displaystyle E$ if $\displaystyle \exists \ x\ \in \ E$ such that $\displaystyle x\ \nexists \ A$.

## 3 Definition - part
$\displaystyle P( E)$ means '*part of $\displaystyle E$*': the set or the subsets of $\displaystyle E$.

> [!Example] Example
> $\displaystyle E=\{1,2,3\} .$
> 
$\displaystyle P( E) =\{\{1\} ,\{2\} ,\{3\} ,\{1,2\} ,\{1,3\} ,\{2,3\} ,\{1,2,3\} ,\ \{\emptyset \}\}$

We form subsets of a set $E$ by selecting or **not selecting** elements from $E$. The empty set has no elements, so it is a subset of any set.

## 4 Unions and intersections

### 4.1 Proposition - intersection included in union
($\displaystyle A\cap B) \in ( A\cup B)$

### 4.2 Proposition
If $\displaystyle A$ is a set, $\displaystyle i$ its index, and $\displaystyle E$ the whole set:
	- $\displaystyle \cup A_{i} \ =\ \{x\in E, \exists i\ ,x\ \in A_{i}\}$
	- $\displaystyle \cap A_{i} \ =\ \{x\ \in E,\ x\in A_{i} ,\ \forall \ i\}$

### 4.3 Definition - the neutral element
The **neutral element**:
$\displaystyle A\cup \emptyset =A$
$\displaystyle A\cap E=A$
With $\displaystyle \emptyset$ the empty set and $\displaystyle E$ the whole set.

### 4.4 Property - associativity
$\displaystyle ( A\cup B) \cup C\ =\ A\cup ( B\cup C) \ =\ A\cup B\cup C$ 

$\displaystyle ( A\cap B) \cup C\ =\ A\cap ( B\cap C) \ =\ A\cap B\cap C$ 

### 4.5 Property - commutativity
$\displaystyle A\cap B\ =\ B\cap A$

$\displaystyle A\cup B=B\cup A$

### 4.6 Property - distributivity
$\displaystyle A\cup ( B\cap C) \ =\ ( A\cup B) \cap ( A\cup C)$
  
## 5 Complementary set

### 5.1 Definition - complementary set
The complementary set of $A$ in $E$ is:
$\displaystyle \complement _{E} A=\{x\in E,\ x\ \notin \ A\ \}$

### 5.2 Proposition - complement of a complement

$\displaystyle \complement _{E} \complement _{E} A=A$

### 5.3 Proposition - complement of empty set

$\displaystyle \complement _{E} \emptyset \ =\ E$

### 5.4 Proposition - complement of whole set

$\displaystyle \complement _{E} E=\emptyset$

### 5.5 Proposition

$\displaystyle ( A\in B) \Longleftrightarrow ( \complement _{E} B\in \complement _{E} A)$

#### 5.5.1 Proof

**$\displaystyle ( A\in B) \implies ( \complement _{E} B\in \complement _{E} A)$**

$\displaystyle \complement _{E} B$ does not belong $\displaystyle B$, so it is not included in $\displaystyle A$ since $\displaystyle A\in B$. Thus it belongs to the complement of $\displaystyle A$, $\displaystyle \complement _{E} A$.

**$\displaystyle ( \complement _{E} A\in \complement _{E} B) \Longrightarrow ( B\in A)$**

Using what we just proved, it is possible to say that $\displaystyle ( \complement _{E} A\in \complement _{E} B) \Longrightarrow ( \complement _{E} \complement _{E} B\in \complement _{E} \complement _{E} A)$. According to [[Sets#5.2 Proposition - complement of a complement]], we deduce that $\displaystyle ( \complement _{E} A\in \complement _{E} B) \Longrightarrow ( B\in A)$.

### 5.6 Definition - disjoint sets

$\displaystyle A$ and $\displaystyle B$ are disjoint if $\displaystyle A\cap B=\emptyset$.

### 5.7 Definition - partition

$\displaystyle A$ and $\displaystyle B$ are a partition of $\displaystyle E$ if :
- they are [[Sets#5.6 Definition - disjoint sets|disjoint]]
- $\displaystyle A\cup B=E$

> [!Example] Example
> $\displaystyle E=\mathbb{N} ,\ A=\left\{\text{odd numbers}\right\} ,\ B=\left\{\text{even numbers}\right\}$

## 6 Cartesian Product

### 6.1 Definition - cartesian product

The **cartesian product** of two sets $\displaystyle E$ and $\displaystyle F$ is the set of all ordered pairs $\displaystyle ( a,\ b)$ where $\displaystyle a$ is in $\displaystyle E$ and $\displaystyle b$ is in $\displaystyle F$:  $\displaystyle E\times F=\{( a,b) ,\ a\in E,\ b\in F\}$

> [!Note] Note
>
> - $\displaystyle ( a,b) \in E\times F$
> - $\displaystyle \{a,b\} \in E\cup F$
> 

If $\displaystyle E=F$ then $\displaystyle E\times F=E^{2}$.

> [!Example] Example
> $\displaystyle E=\mathbb{R} ,\ E\times E=\mathbb{R}^{2}$, wich defines the cartesian plane formed by all the possible ordered pairs $\displaystyle ( x,y)$.

## 7 Applications

### 7.1 Definition - application

Being given two sets $\displaystyle E$ and $\displaystyle F$, one defines an **application** from $\displaystyle E$ to $\displaystyle F$ if, **to each element** $\displaystyle a\in E$, one associates an element $\displaystyle b$ of $\displaystyle F$ such that $\displaystyle b=f( a)$.

### 7.2 Definition - image and antecedent

Given $\displaystyle a$ the **antecedent**, $\displaystyle b$ the **image**.
The image of a subset $\displaystyle A$ of $\displaystyle E$ is $\displaystyle B=f( A) =\{b=f( a) ,\ a\ \in E\}$

### 7.3 Definition - reciprocal image of a subset

The **reciprocal image** of a subset $\displaystyle B$ of $\displaystyle F$ is $\displaystyle f^{-1}( B) =A=\{a\in E,\ f( a) \in B\}$

> [!Example] Example
> $\displaystyle f( x) =|x|,\ \mathbb{R\rightarrow R}$
> 
> $\displaystyle f(\mathbb{R}) =\mathbb{R}^{+} =\{x\in \mathbb{R} ,x\geqslant 0\}$
> 
> $\displaystyle f^{-1}\left(\mathbb{R}^{+}\right) =\mathbb{R}$

### 7.4 Definition - injective
$\displaystyle f$ is said to be **injective** if each element of $\displaystyle F$ has at most one antecedent in $\displaystyle E$.

> [!Example] Example
> 
> $\displaystyle E=\mathbb{R} ,\ F=\mathbb{R} ,\ f( x) =|x|$ is not a bijection from $\displaystyle E$ to $\displaystyle F$ since an an element of $\displaystyle F$ may have two antecedents in $\displaystyle E$. Though, it is a bijection from $\displaystyle E=\mathbb{R}^{+}$ to $\displaystyle F=\mathbb{R}^{+}$and also from $\displaystyle E=\mathbb{R}^{+}$ to $\displaystyle F=\mathbb{R}$.

### 7.5 Proposition
If $\displaystyle g$ and $\displaystyle f$ are both injective, and $\displaystyle g( x) =g( y)$ then $\displaystyle x=y$.

### 7.6 Definition - subjective
$\displaystyle f$ is said to be **subjective** if each element of $\displaystyle F$ has at least one antecedent in $\displaystyle E$. So, by definition,$\displaystyle f( E) =F$.

### 7.7 Definition - bijective
$\displaystyle f$ is said to be an **bijective** if it is both subjective and injective, thus, each element of $\displaystyle F$ has one and only one antecedent in $\displaystyle E$.

> [!Example] Example
> $\displaystyle f( x) =|x|$
> 
> $\displaystyle f:\mathbb{R\rightarrow R}$: nor subjective or bijective
> 
> $\displaystyle f:\mathbb{R\rightarrow R}^{+}$: subjective
> 
> $\displaystyle f:\mathbb{R}^{+}\rightarrow \mathbb{R}^{+}$: bijective

### 7.8 Proposition
Given an application $\displaystyle f$. $\displaystyle f$ is not subjective. If we restrict the image set to $\displaystyle f( E)$, then it becomes subjective from $\displaystyle E$ to $\displaystyle f( E)$.

> [!Example] Example
> $\displaystyle f( x) =|x|$
> 
> $\displaystyle f:\mathbb{R\rightarrow R}$
> 
> $\displaystyle f( x)$ is an application because each element of $\displaystyle E$ has at least image in $\displaystyle F$. It is not subjective. Though, if we restric the image set to $\displaystyle f( E) =\mathbb{R}^{+}$, then it becomes subjective as, for each element of $\displaystyle F$, there is at least one element of $\displaystyle E$.

## 8 Composition of applications

Given $\displaystyle E,\ F,\ G$ three sets:
- $\displaystyle f$ goes from $\displaystyle E$ to $\displaystyle F$, and $\displaystyle g$ goes from $\displaystyle F$ to $\displaystyle G$.
- $\displaystyle \forall a\in E,\ b=f( a) \in F,\ c=g( b) \ \in G$

### 8.1 Definition - composition of applications
$\displaystyle ( g\circ f)( x) \ =\ g( f( x))$

$\displaystyle ( g\circ f) :\ E\rightarrow G$

### 8.2 Property - associativity
$\displaystyle h\circ g\circ f=h\circ ( g\circ f) =( h\circ g) \circ f$

#### 8.2.1 Proof 
$\displaystyle ( h\circ g\circ f)( x) =h( g( f( x)) =( h\circ g)( f( x)) =h\circ ( g\circ f( x))$

### 8.3 Proposition - composition of injections
The composition of injections is also an injection.

#### 8.3.1 Proof
Suppose that $\displaystyle g$ and $\displaystyle f$ are injectives and $\displaystyle ( g\circ f)( x) =( g\circ f)( y)$.

So $\displaystyle g( f( x)) =g( f( y))$

Since $\displaystyle g$ is injective, it implies that one image $\displaystyle ( g( f( x)) ,\ g( f( y)))$ can have at most one antecedent.  so $\displaystyle f( x)$ must be equal to $\displaystyle f( y)$.

Besides, $\displaystyle f$ is also injective so $\displaystyle x$ must be equal to $\displaystyle y$.

Conclusion: $\displaystyle ( g\circ f)( x) =( g\circ f)( y) \Longrightarrow x=y\ \Longrightarrow \ g\circ f$ is injective.

### 8.4 Proposition - composition of subjections
The composition of subjections is also a subjection.

#### 8.4.1 Proof
$\displaystyle f$ subjective $\displaystyle \Longrightarrow f( E) =F$
$\displaystyle g$ subjective $\displaystyle \Longrightarrow g( F) =G$
Wich implies that $\displaystyle g( f( E)) =( g\circ f)( E) =G$
Wich implies that $\displaystyle ( g\circ f)$ is subjective.

### 8.5 Proposition - composition of bijections
The composition of bijections is also a bijection.

### 8.6 Proposition - injection to bijection
An injection is a bijection from $\displaystyle E$ to its image set $\displaystyle f( E)$.

> [!Example] Example
> $\displaystyle f( x) =|x|$
> 
> $\displaystyle f:\mathbb{R\rightarrow R}^{+}$
> 
> $\displaystyle E=\mathbb{R} ,\ f( E) =\mathbb{R}^{+}$

## 9 Restriction and extension of an application
$\displaystyle f:\ E\rightarrow F,\ A\in E$

### 9.1 Defintion - restriction and extension
The restriction of $\displaystyle f$ to $\displaystyle A$ is an application $\displaystyle f$ from $\displaystyle A$ to $\displaystyle F$ such that $\displaystyle \varphi ( x) =f( x) ,\ \forall x\in A$. 
We can say that $\displaystyle f$ is an extension of $\displaystyle \varphi $ to the whole space $\displaystyle E$.

> [!Example] Example
> $\displaystyle \varphi ( x) =\left(\sqrt{x-1}\right)^{2}$
> 
> $\displaystyle \varphi$ is defined on $\displaystyle A=[ 1,+\infty [$
> 
> The extension of $\displaystyle \varphi$ to $\displaystyle \mathbb{R}$ is $\displaystyle f( x) =x-1$ because $\displaystyle f( x) =\varphi ( x)$ on $\displaystyle A$.
> 
> $\displaystyle \varphi :A\rightarrow \mathbb{R}$
> 
> $\displaystyle f:\mathbb{R}\rightarrow \mathbb{R}$

## 10 Binary relations

### 10.1 Definition - binary relation

Giving a **binary relation** on $\displaystyle E$ consists in introducing a partition of $\displaystyle E\times E$ in two subsets $\displaystyle G$ and $\displaystyle G'$ such that $\displaystyle aRb\Longleftrightarrow ( a,b) \in G,\ G$ being the graph of $R$, and $R$ being a binary relationship.

> [!Example] Example
> $\displaystyle a\in \mathbb{R}, b\ \in \mathbb{R}^{+} ,\ a\leqslant b$
> ![[diagram-20230502.svg]] 

### 10.2 Property - reflexivity ($\mathcal{R}$)

A binary relationship $R$ is **reflexive** if  $\displaystyle aRa,\ \forall a\in E$. Geometrically, it means that the first bisectrix is included in $\displaystyle G$.

> [!Example] Example
> $\displaystyle a\leqslant b$ is reflexive since $\displaystyle a\leqslant a$.

### 10.3 Property - symmetry
A binary relationship $\displaystyle R$ is **symmetric** if  $\displaystyle aRb\Longrightarrow bRa$. So, if $\displaystyle ( a;b)$ belongs to $\displaystyle G$, then $\displaystyle ( b;a)$ also belongs to $\displaystyle G$. Geometrically, it means that the graph $\displaystyle G$ is symmetric with respect to the first bisectrix. 

### 10.4 Property - antisymmetry ($\mathcal{A}$)
$\displaystyle \begin{drcases}
G=aRb\\
G=bRa
\end{drcases} \Longrightarrow a=b$

> [!Example] Example
> $\displaystyle a\leqslant b$
> 
> So, $\displaystyle a\leqslant b$ and $\displaystyle b\leqslant a$ implies that $\displaystyle a=b$.
> 

### 10.5 Property - transitivity ($\mathcal{Z}$)
$\displaystyle \begin{drcases}
G=aRb\\
G=bRc
\end{drcases} \Longrightarrow G=aRb$

> [!Example] Example
> $\displaystyle a\leqslant b$
> 
> So $\displaystyle a\leqslant b$ and $\displaystyle b\leqslant c$ implies that $\displaystyle a\leqslant c$.