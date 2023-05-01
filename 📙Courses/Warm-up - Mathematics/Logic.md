# Logic

## 1 Logical symbols

| Symbol                | Description         |
| --------------------- | ------------------- |
| $\implies$            | implies             |
| $\nRightarrow$        | not implies         |
| $\Longleftrightarrow$ | logical equivalence |
| $\forall$             | for all             |
| $\exists$             |         there exists at least one            |
| $\exists!$            |  there exists one and only one                 |
| $\nexists$                      |    there does not exist                 |

Exemple: $\forall x \in \mathbb{R}, \exists! y \in \mathbb{R} \text{ such that } x+y=0$

### 1.1 Proposition

>$$\displaystyle ( A) \ \Longrightarrow \ ( B) \ \Longleftrightarrow \ \left(\not{B}\right) \Longrightarrow \left(\not{A}\right)$$

#### 1.1.1 Proof

Suppose we have $\displaystyle \left(\not{B}\right)$ ($\displaystyle B$ is not satisfied). If $\displaystyle ( A)$ then $\displaystyle ( B)$, wich is in contradiction with our supposition, thus $\displaystyle \left(\not{B}\right) \Longrightarrow \left(\not{A}\right)$.

#### 1.1.2 Negation

Proposition: $\displaystyle \forall x,\ ( P)$ is satisfied 
Negation: $\displaystyle \exists x,\ ( P)$ is not satisfied

> [!NOTE] Note - Why isn't the negation: $\displaystyle \forall x,\ ( P)$ is not satisfied?
> The negation of a proposition means that we inverse its truth value. To negate our present proposition, it is only needed to find one $\displaystyle x$ where $\displaystyle ( P)$ isn't satisfied to prove it false.



