**5.2 Vector spaces**

We recollect that for a non-empty set $G$, a binary operation on $G$ is mapping from $G \times G$ into $G$.

**Definition:** A non-empty set $G$ together with a binary operation $*$ is called a **group** if the algebraic system $(G, *)$ satisfies the following four axioms:

(i) $\underline{\text{Associative axiom}}$: $(a * b) * c = a * (b * c)$ for all elements $a, b, c \in G$.

(ii) $\underline{\text{Identity axiom}}$: There exists an element $e \in G$ such that $a * e = e * a = a$ for all elements $a \in G$.

(iii) $\underline{\text{Inverse axiom}}$: To each element $a \in G$ there corresponds an element $b \in G$ such that $a * b = e = b * a$.

Moreover $G$ is said to be **abelian** if $a * b = b * a$ for all $a, b \in G$ (similarly, $G$ is commutative if the multiplication $a \cdot b = b \cdot a$ for all $a, b \in G$).

**Examples:** (i) The set of all integers with respect to addition is an abelian group.

(ii) The set of all $2 \times 2$ matrices with real or complex entries is a group with respect to matrix addition.

**Definition:** A non-empty set $F$ is said to be a **field** if there exists two binary operations $+$ and "$\cdot$" on $F$ such that

(i) $(F, +)$ is an abelian group
(ii) $(F \setminus \{0\}, \cdot)$ is a multiplicative group and
(iii) for any $a, b, c \in F$, we have $a(b + c) = ab + ac$, $(a + b)c = ac + bc$.

**Examples:** (i) Set of real numbers with usual addition and multiplication is a field.

(ii) The set of all complex numbers is also a field with respect to the addition and multiplication of complex numbers.

**Definition:** A non-empty set $V$ is said to be a *vector space* over a field $F$ (generally, we take the field as the set of real numbers or the set of complex numbers) if it satisfying the following:

(i) $(V, +)$ is an abelian group,

(ii) $V$ is closed under scalar multiplication (that is, for every $\alpha \in F$, $v \in V$ we have $\alpha v \in V$) and also this scalar multiplication satisfies the following conditions:

(a) $\alpha(v + w) = \alpha v + \alpha w$,

(b) $(\alpha + \beta)v = \alpha v + \beta v$,

(c) $\alpha(\beta v) = (\alpha\beta)v$ and

(d) $1.v = v$ for all $\alpha, \beta \in F$ and $v, w \in V$ (here $1$ is the identity of $F$ with respect to multiplication).

Here $+$ is addition either in the field or in the vector space, as appropriate; and $0$ is the additive identity in either. Juxtaposition indicates either scalar multiplication or the multiplication operation in the field.

*Note: We use $F$ for field, also the elements of $F$ are called scalars and the elements of $V$ are called vectors.*

**Definition:** (i) An n-component vector **a** is an ordered n-tuple of numbers written as a row $(a_1, \dots, a_n)$ or as a column $\begin{pmatrix} a_1 \\ a_2 \\ \vdots \\ a_n \end{pmatrix}$ where $a_i$, $i = 1, 2, \dots, n$ are assumed to be real numbers and are called the components of the vector.

(ii) A unit vector denoted by $e_i$ and defined with unity as value of its $i^{\text{th}}$ component and all other components zero.

(iii) Null vector is a vector all of whose components are zero.

(iii) A sum vector is a vector having unity as a value for each component; it will be written as 1.

(iv) Let $\mathbf{a}$ and $\mathbf{b}$ be two n-component vectors. Then $\mathbf{a}$ and $\mathbf{b}$ are equal if and only if $a_i = b_i$ for each $i$.

(v) The scalar product of two n-component vectors $\mathbf{a}$, $\mathbf{b}$ is defined to be the scalar $a_1b_1 + a_2b_2 + \dots + a_nb_n = \sum_{i=1}^{n} a_i b_i$.

**Definition:** The norm of an n-component vector $\mathbf{a} = (a_1, a_2, \dots, a_n)$ is denoted and defined by $\|\mathbf{a}\| = \sqrt{\langle\mathbf{a}, \mathbf{a}\rangle} = \sqrt{a_1^2 + a_2^2 + \dots + a_n^2}$.

**Euclidean Space:** An n-dimensional Euclidean space is defined as the collection of all vectors (points) $\mathbf{a} = (a_1, a_2, \dots, a_n)$. For these vectors, addition and multiplication by a scalar are defined as follows.

$$E^n = \{(a_1, a_2, \dots, a_n) \mid \text{each } a_i \text{ is a real or complex number}, 1 \leq i \leq n\}$$

Define addition and multiplication by scalar in $E^n$ as, for any

$$(a_1, a_2, \dots, a_n), (b_1, b_2, \dots, b_n) \in E^n$$

$$(a_1, a_2, \dots, a_n) + (b_1, b_2, \dots, b_n) = (a_1 + b_1, a_2 + b_2, \dots, a_n + b_n) \in E^n \text{, and for any scalar } \lambda$$

$$\lambda(a_1, a_2, \dots, a_n) = (\lambda a_1, \lambda a_2, \dots, \lambda a_n) \in E^n$$

Therefore $E^n$ is a vector space (over $\mathbb{R}$).

**18.2.22 Example:** Let $M_{2 \times 2} = \left\{ \begin{pmatrix} a_1 & a_2 \\ a_3 & a_4 \end{pmatrix} \;\middle|\; a_i \text{ is a real number} \right\}$. Then $M_{2 \times 2}$ is a vector space over the set of real numbers, with respect to the addition of matrices and the multiplications of a matrix by a scalar.

**Definition:** Let $V$ be a vector space over $F$ and $W \subseteq V$. Then $W$ is called a *subspace* of $V$ if $W$ is a vector space over $F$ under the same operation.

**Definition:** Suppose $V$ is a vector space over $F$, $v_i \in V$ and $\alpha_i \in F$ for $1 \leq i \leq n$. Then

$$\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_n v_n$$

is called the *linear combination* (over $F$) of $\{v_1, v_2, \dots, v_n\}$.

**Definition:** Let $V$ be a vector space and $S \subseteq V$. We write

$$L(S) = \{\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_n v_n / n \in \mathbb{N}, v_i \in S \text{ and } \alpha_i \in F \text{ for } 1 \leq i \leq n\}$$

which is equal to the set of all linear combinations of finite number of elements of $S$. This $L(S)$ is called the *linear span of $S$*.

**Example:** Let $\mathbf{a} = (2, 3, 4, 7)$, $\mathbf{b} = (0, 0, 0, 1)$, $\mathbf{c} = (1, 0, 1, 0)$. Then the vector $\mathbf{d} = (5, 3, 7, 9)$ is a linear combination of the vectors $\mathbf{a}$, $\mathbf{b}$, $\mathbf{c}$ as follows:

$$(5, 3, 7, 9) = (2, 3, 4, 7) + 2(0, 0, 0, 1) + 3(1, 0, 1, 0)$$

**18.2.19 Example:** Let the field $K$ be the set $\mathbf{R}$ of real numbers, and let the vector space $V$ be the Euclidean space $\mathbf{R}^3$. Consider the vectors $e_1 := (1,0,0)$, $e_2 := (0,1,0)$ and $e_3 = (0,0,1)$. Then any vector in $\mathbf{R}^3$ is a linear combination of $e_1$, $e_2$ and $e_3$.

**Note:** Let $v \in S$. Then $1 \cdot v$ is a linear combination and hence $v \in L(S)$. Therefore, $S \subseteq L(S)$.

**Problem:** *Let $V$ be a vector space over $F$ and $\phi \neq W \subseteq V$. Then the following two conditions are equivalent. (i) $W$ is a subspace of $V$*
$$(ii)\ \alpha, \beta \in F \text{ and } w_1, w_2 \in W \Rightarrow \alpha w_1 + \beta w_2 \in W.$$

**Example:** The set $S_{2 \times 2} = \left\{ \begin{pmatrix} a & a \\ a & a \end{pmatrix} \Big/ a \text{ is a real number} \right\}$ is a subspace of $M_{2 \times 2}$.

**Example:** The set $W = \{\alpha(1, 1, 0) \mid \alpha \text{ is a real number}\}$ is a subspace of $\mathbf{R}^3$.

**Problem:** *If $S$ is any subset of a vector space $V$, then show that $L(S)$ is a subspace of $V$.*

**Solution:** Let $v, w \in L(S)$ and $\alpha, \beta \in F$. Since
$$v, w \in L(S),$$
we have that
$$v = \alpha_1 v_1 + \dots + \alpha_n v_n \text{ and } w = \beta_1 w_1 + \dots + \beta_m w_m$$
for some $v_i \in S$, $\alpha_i \in F$ for $1 \le i \le n$ and $w_j \in S$, $\beta_j \in F$ for $1 \le j \le m$. Now
$$\alpha v + \beta w$$
$$= \alpha(\alpha_1 v_1 + \dots + \alpha_n v_n) + \beta(\beta_1 w_1 + \dots + \beta_m w_m)$$
$$= \alpha \alpha_1 v_1 + \alpha \alpha_2 v_2 + \dots + \alpha \alpha_n v_n + \beta \beta_1 w_1 + \beta \beta_2 w_2 + \dots + \beta \beta_m w_m,$$
is a linear combination of elements from $S$.

Hence $\alpha v + \beta w \in L(S)$. This shows that $L(S)$ is a subspace of $V$.

---

***Properties of linear span:*** *If $S$ and $T$ are subsets of a vector space $V$ then*

*(i) $S \subseteq T \Rightarrow L(S) \subseteq L(T)$,*

*(ii) $L(S \cup T) = L(S) + L(T)$,*

*(iii) $L(L(S)) = L(S)$.*

**Definitions:** (i) The vector space $V$ is said to be ***finite-dimensional*** (over $F$) if there is a finite subset $S$ in $V$ such that $L(S) = V$.

(ii) The vectors $v_i \in V$ for $1 \le i \le n$, are ***linearly dependent*** over $F$ if there exists elements $a_i \in F$, $1 \le i \le n$, $\underline{\text{not all of them equal to zero}}$, such that $a_1 v_1 + a_2 v_2 + \dots + a_n v_n = 0$. If the vectors $v_i$, $1 \le i \le n$ are not linearly dependent over $F$ then they are said to be ***linearly independent*** *over $F$.*

**Examples:** Consider $R$, the set of real numbers and take $V = R^2$, then

*(i) $V$ is vector space over the field $R$.*

(ii) Consider $S = \{(1, 0), (1, 1), (0, 1)\} \subseteq R^2$. Then the linear span of $S$ is
$$L(S) = \{\alpha_1(1, 0) + \alpha_2(1, 1) + \alpha_3(0, 1) / \alpha_i \in R, 1 \le i \le 3\}$$
$$= \{(\alpha_1 + \alpha_2, \alpha_2 + \alpha_3) / \alpha_i \in R, 1 \le i \le 3\} \subseteq R^2.$$
If $(x, y) \in R^2$ then write $\alpha_1 = x$, $\alpha_2 = 0$, $\alpha_3 = y$ then
$(x, y) = (\alpha_1 + \alpha_2, \alpha_2 + \alpha_3) \in L(S)$. Hence $L(S) = R^2 = V$.

This shows that $R^2$ is finite dimensional.

(iii) Write $v_1 = (1, 0)$, $v_2 = (2, 2)$, $v_3 = (0, 1)$, $v_4 = (3, 3)$. Then
$$\alpha_1 v_1 + \alpha_2 v_2 + \alpha_3 v_3 + \alpha_4 v_4 = \mathbf{0} \text{ where } \alpha_1 = 2, \alpha_2 = -1, \alpha_3 = 2, \alpha_4 = 0.$$
Thus there exists scalars $\alpha_1, \alpha_2, \alpha_3, \alpha_4$ not all of them equal to zero such that
$$\alpha_1 v_1 + \alpha_2 v_2 + \alpha_3 v_3 + \alpha_4 v_4 = \mathbf{0}.$$
Hence $\{v_i / 1 \le i \le 4\}$ is a linearly dependent set.

(iv) Suppose $v_1 = (1, 0)$, $v_2 = (0, 1)$. Suppose $\alpha_1 v_1 + \alpha_2 v_2 = 0$ for some $\alpha_1, \alpha_2 \in R$. Then

$$\alpha_1(1, 0) + \alpha_2(0, 1) = \mathbf{0} = (0, 0)$$
$$\Rightarrow (\alpha_1, \alpha_2) = (0, 0)$$
$$\Rightarrow \alpha_1 = 0 = \alpha_2.$$

Hence $v_1, v_2$ are linearly independent.

***Lemma:*** *Let $V$ be a vector space over $F$. If $v_1, v_2, \dots, v_n \in V$ are linearly independent, then every element in their linear span has a unique representation in the form $\lambda_1 v_1 + \lambda_2 v_2 + \dots + \lambda_n v_n$ with $\lambda_i \in F, 1 \le i \le n$.*

**Proof:** Let $S = \{v_i / 1 \le i \le n\}$. Consider $L(S)$. Let $v \in L(S)$. Then
$$v = \alpha_1 v_1 + \dots + \alpha_n v_n$$
for some $\alpha_i \in F$, $v_i \in S$, $1 \le i \le n$ (by the definition of $L(S)$).

Uniqueness: Suppose $v = \alpha_1 v_1 + \dots + \alpha_n v_n = \beta_1 v_1 + \dots + \beta_n v_n$ for some $\alpha_i, \beta_i \in F, \quad 1 \le i \le n$
$$\Rightarrow (\alpha_1 v_1 + \dots + \alpha_n v_n) - (\beta_1 v_1 + \dots + \beta_n v_n) = 0$$
$$\Rightarrow (\alpha_1 - \beta_1) v_1 + \dots + (\alpha_n - \beta_n) v_n = 0$$
$$\Rightarrow \alpha_1 - \beta_1 = 0, \alpha_2 - \beta_2 = 0, \dots, \alpha_n - \beta_n = 0 \text{ (since } v_i, 1 \le i \le n \text{ are linearly independent)}$$
$$\Rightarrow \alpha_1 = \beta_1, \alpha_2 = \beta_2, \dots, \alpha_n = \beta_n.$$

Hence every element in the linear span can be expressed as in a unique way as a linear combination of $v_i, 1 \le i \le n$.

***Theorem:*** *If $v_i \in V, 1 \le i \le n$, then either they are linearly independent or some $v_k$ is a linear combination of the preceding ones $v_1, v_2, \dots, v_{k-1}$.*

**Proof:** If $v_i, 1 \le i \le n$ are linearly independent then there is nothing to prove. Suppose that $v_i, 1 \le i \le n$ are $\underline{\text{not linearly independent}}$ (that is, linearly dependent). Then there exist scalars $\alpha_i, 1 \le i \le n$ $\underline{\text{not all zero}}$, such that
$$\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_n v_n = \mathbf{0}.$$
Since all the $\alpha_i$ are not zero, there exists largest $k$ such that $\alpha_k \neq 0$. Then

---

$$\alpha_{k+1} = 0, \dots, \alpha_n = 0 \text{ and so } \alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_k v_k = \mathbf{0}$$
$$\Rightarrow \alpha_k v_k = -\alpha_1 v_1 - \alpha_2 v_2 - \dots - \alpha_{k-1} v_{k-1}$$
$$\Rightarrow v_k = \alpha_k^{-1}(-\alpha_1 v_1 - \alpha_2 v_2 - \dots - \alpha_{k-1} v_{k-1}) = -\alpha_k^{-1}\alpha_1 v_1 - \dots - \alpha_k^{-1}\alpha_{k-1} v_{k-1} \text{ and }$$
$$\alpha_k^{-1}\alpha_i \in F \text{ for each } 1 \le i \le k-1.$$

Hence $v_k$ is a linear combination of $v_i, 1 \le i \le k-1$.

**Definition:** *A subset $S$ of a vector space $V$ is called a **basis** of $V$ if*

*(i) $S$ consists of linearly independent elements (that is, any finite number of elements in $S$ is a linearly independent), and*

*(ii) $S$ spans $V$ (that is, $V = L(S)$).*

**Note:** A subset $B$ of a vector space is a basis $\underline{\text{if and only if}}$ any of the following equivalent conditions are met:

* $B$ is a minimal generating set of $V$, i.e., it is a generating set but no $\underline{\text{proper subset}}$ $\underline{\text{of } B \text{ is}}$.
* $B$ is a maximal set of linearly independent vectors, i.e., it is a linearly independent set but no other linearly independent set contains it as a proper subset.
* Every vector in $V$ can be expressed as a linear combination of vectors in $B$ in a unique way.

**Examples:**

(i) Consider $\mathbf{R}^2$, the vector space of all coordinates $(a, b)$ where both $a$ and $b$ are real numbers.

Then a very natural and simple basis is simply the vectors $\mathbf{e_1} = (1,0)$ and $\mathbf{e_2} = (0,1)$: suppose that $v = (a, b)$ is a vector in $\mathbf{R}^2$, then $v = a(1,0) + b(0,1)$.

(ii) The set of vectors $\{(1, 1), (-1, 2)\}$ form a basis of $\mathbf{R}^2$.

Verification: Part (i): First we prove that $\{(1, 1), (-1, 2)\}$ is a linearly independent set.

Suppose that there are numbers $a$, $b$ such that: $a(1, 1) + b(-1, 2) = (0, 0)$.

$\Rightarrow (a - b, a + 2b) = (0, 0) \Rightarrow a - b = 0$ and $a + 2b = 0$. Subtracting we get $3b = 0$ and so $b = 0$. From the first equation we get that $a = 0$.

Part (ii): In this part we show that $\{(1, 1), (-1, 2)\}$ generates $\mathbb{R}^2$. Let $(a, b) \in \mathbb{R}^2$. Now we show that there exists two numbers $x$ and $y$ such that

$x(1, 1) + y(-1, 2) = (a, b)$. Then we have to solve the equations:

$x - y = a$ and $x + 2y = b$

Subtracting the first equation from the second, we get $3y = b - a \Rightarrow y = (b - a)/3$ and $x = (b + 2a)/3$. Therefore $\{(1, 1), (-1, 2)\}$ generates (or spans) $\mathbf{R}^2$.

Observation:

(i) Since $(-1, 2)$ is clearly not a multiple of $(1, 1)$ and since $(1, 1)$ is not the zero vector, these two vectors are linearly independent. Since the dimension of $\mathbf{R}^2$ is $2$, the two vectors already form a basis of $\mathbf{R}^2$ without needing any extension.

(ii) The standard basis (also called natural basis or canonical basis) of the $n$-dimensional Euclidean space $\mathbf{R}^n$ is the basis obtained by taking the $n$ basis vectors, $(e_1, e_2, \dots, e_n)$ where $e_i$ is the vector with a $1$ in the $i^{\text{th}}$ coordinate and $0$ elsewhere. In many ways, it is the "obvious" basis.

Example: The set of all $n$ unit vectors $e_1, e_2, \dots, e_n$ form a basis for $\mathbb{R}^n$.

To show that the set $\{e_1, e_2, \dots, e_n\}$ is linearly independent:

Suppose $\alpha_1 e_1 + \alpha_2 e_2 + \dots + \alpha_n e_n = \mathbf{0}$.

This means: $\alpha_1(1, 0, \dots, 0) + \alpha_2(0, 1, 0, \dots, 0) + \dots + \alpha_n(0, 0, \dots, 1) = (0, 0, \dots 0)$.

$\Rightarrow (\alpha_1, 0, \dots, 0) + (0, \alpha_2, \dots, 0) + \dots + (\alpha_n, \dots, 1) = (0, 0, \dots, 0)$.

$\Rightarrow (\alpha_1, \alpha_2, \dots, \alpha_n) = (0, 0, \dots, 0)$.

This means that $\alpha_1 = 0, \alpha_2 = 0, \dots, \alpha_n = 0$.

Therefore $\{e_1, e_2, \dots, e_n\}$ is linearly independent.

Next to show that $\{e_1, e_2, \dots, e_n\}$ spans $\mathbb{R}^n$. Let $\mathbf{x} = (x_1, x_2, \dots, x_n) \in \mathbb{R}^n$. Then $\mathbf{x}$ can be represented as a linear combination of $\{e_1, e_2, \dots, e_n\}$ in the following way.

$$\mathbf{x} = x_1 e_1 + x_2 e_2 + \dots + x_n e_n$$

Therefore the set $\{e_1, e_2, \dots, e_n\}$ spans $\mathbb{R}^n$ and hence a basis.

Example: Prove that the set $B = \left\{ \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}, \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}, \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix}, \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} \right\}$ is a basis for $M_{2 \times 2}$.

Solution: The set $B$ is linearly Independent:

Suppose $\alpha_1 \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + \alpha_2 \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} + \alpha_3 \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} + \alpha_4 \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$. This implies that $\alpha_1 = 0$, $\alpha_2 = 0, \alpha_3 = 0, \alpha_4 = 0$.

We show that the set $B$ spans $M_{2 \times 2}$:

Let $\begin{pmatrix} a & b \\ c & d \end{pmatrix} \in M_{2 \times 2}$. Then

$$\begin{pmatrix} a & b \\ c & d \end{pmatrix} = a \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + b \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} + c \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} + d \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} \text{ Therefore the set B spans } M_{2 \times 2}, \text{ and}$$

hence a basis.

**Example:** Test whether the set $B = \{(1, 1, 0), (3, 0, 1), (5, 2, 2)\}$ forms a basis for $\mathbf{R}^3$. If so represent $(1, 2, 3)$ in terms of basis vectors.

**Solution:** Consider the matrix determinant of the coefficients.

$$D = \begin{vmatrix} 1 & 3 & 5 \\ 1 & 0 & 2 \\ 0 & 1 & 2 \end{vmatrix} = 1(-2) - 3(2) + 5(1) = -3 \neq 0$$

Let $(a, b, c) \in \mathbf{R}^3$.
Now $(a, b, c) = \alpha_1(1, 1, 0) + \alpha_2(3, 0, 1) + \alpha_3(5, 2, 2)$
This means 
$$\begin{aligned}
\alpha_1 + 3\alpha_2 + 5\alpha_3 &= a \\
\alpha_1 + 2\alpha_3 &= b \\
\alpha_2 + 2\alpha_3 &= c
\end{aligned}$$

Solving, by Cramer's rule

$$\alpha_1 = \frac{\begin{vmatrix} a & 3 & 5 \\ b & 0 & 2 \\ c & 1 & 2 \end{vmatrix}}{D} = \frac{-2a - b + 6c}{-3}$$

$$\alpha_2 = \frac{\begin{vmatrix} 1 & a & 5 \\ 1 & b & 2 \\ 0 & c & 2 \end{vmatrix}}{D} = \frac{2b - 2a + 3c}{-3} \quad \text{and}$$

$$\alpha_3 = \frac{\begin{vmatrix} 1 & 3 & a \\ 1 & 0 & b \\ 0 & 1 & c \end{vmatrix}}{D} = \frac{a - b + 3c}{-3}$$

when $(a, b, c) = (1, 2, 3)$, we have $\alpha_1 = -14/3$, $\alpha_2 = -11/3$, $\alpha_3 = 10/3$.
Therefore $(1, 2, 3) = -14/3(1, 1, 0) - 11/3(3, 0, 1) + 10/3(5, 2, 2)$.

**Problem:** Any vector in $\mathbf{R}^n$ can be expressed as a linear combination of a set of vectors in only one way.

**Proof:** Let $b \in \mathbf{R}^n$ and $\{a_1, a_2, \dots, a_r\}$ a set of basis vectors.

Suppose that $b$ is expressed in two ways as follows:

$$b = \alpha_1 a_1 + \alpha_2 a_2 + \dots + \alpha_r a_r \quad \text{and} \quad b = \beta_1 a_1 + \beta_2 a_2 + \dots + \beta_r a_r \quad \text{where }\alpha\text{'s and }\beta\text{'s are scalars.}$$

Now $(\alpha_1 - \beta_1)a_1 + (\alpha_2 - \beta_2)a_2 + \dots + (\alpha_r - \beta_r)a_r = 0$.

Since $\{a_1, a_2, \dots, a_r\}$ is linearly independent, we have that

$$\alpha_1 - \beta_1 = \alpha_2 - \beta_2 = \dots = \alpha_r - \beta_r = 0$$

This means $\alpha_1 = \beta_1$, $\alpha_2 = \beta_2, \dots, \alpha_r = \beta_r = 0$.

*Remark: If $V$ is a finite dimensional vector space over $F$, then any two bases of $V$ have that same number of elements.*

**Problem:** Define minimal spanning set of vectors. Prove that a minimal spanning set of vectors forms a basis.

**Solution:**

*Mimimal spanning set:* A subset $S$ of a vector space $V$ is said to be a *minimal spanning set* if (i) $S$ is a spanning set for $V$, and (ii) $S \setminus \{v\}$ do not span $V$ for any $v \in S$.

Let $S = \{v_1, v_2, \dots, v_n\}$ be a minimal spanning set. This means $L(S) = V$.

In order to prove $S$ is a basis, it suffices to prove $S$ is linearly independent.

In a contrary way, suppose that $S$ is not linearly independent.

Then there exists $v_j$ (for some $j$, $1 \le j \le n$) is a linear combination of its preceding ones.

That is.,

$$v_j = \alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_{j-1} v_{j-1} \quad \text{for some } \alpha_i \in F, 1 \le i \le (j - 1)$$

Clearly $L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}) \subseteq L(\{v_i / 1 \le i \le n\}) = L(S)$.

On the other hand, take $x \in L(S)$.

Then $x = \beta_1 v_1 + \beta_2 v_2 + \dots + \beta_n v_n$ for some $\beta_i \in F$, $1 \le i \le n$

$$\Rightarrow x = \beta_1 v_1 + \dots + \beta_{j-1} v_{j-1} + \beta_j(\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_{j-1} v_{j-1}) + \beta_{j+1} v_{j+1} + \dots + \beta_n v_n$$

$$\Rightarrow x = (\beta_1 + \beta_j \alpha_1) v_1 + \dots + (\beta_{j-1} + \beta_j \alpha_{j-1}) v_{j-1} + \beta_{j+1} v_{j+1} + \dots + \beta_n v_n$$

$$\in L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}).$$

Therefore, $L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}) = L(S) = V$, which is a contradiction to the fact that $n$ is minimum with $S$ spans $V$. Therefore $S$ is linearly independent.

**Problem:** Define a maximal linearly independent set. Prove that a maximal linearly independent set is a basis.

**Solution:**

*Maximal linearly independent set:* A subset $S$ of a vector space $V$ is said to be a *maximal linearly independent set* if (i) $S$ is a linearly independent set, and (ii) $S \cup \{v\}$ is linearly dependent for any $v \in V \setminus S$.

Let $S = \{v_1, v_2, \dots, v_n\}$ be a maximal linearly independent set. In order to prove $S$ is a basis, it suffices to prove $S$ spans $V$.

Take $v \in V$. Suppose $\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_n v_n + \alpha v = 0$.

If $\alpha = 0$, then since $v_1, v_2, \dots, v_n$ are linearly independent, we get $\alpha_i = 0$ for all $1 \le i \le n$. This means $v, v_1, v_2, \dots, v_n$ are (which are $n + 1$, in number) linearly independent, a contradiction to the maximality of $n$.

Therefore, $\alpha \neq 0$. Now $\alpha v = (-\alpha_1 v_1) + (-\alpha_2 v_2) + \dots + (-\alpha_n v_n)$.

This implies $v = (-\alpha_1 \alpha^{-1}) v_1 + (-\alpha_2 \alpha^{-1}) v_2 + \dots + (\alpha_n \alpha^{-1}) v_n$.

Therefore $S$ spans $V$. Hence $S$ is a basis.

**Problem 2:** Whether the vectors $\{a_1 = (4, 2, 1), a_2 = (2, -6, -5), a_3 = (1, -2, 3)\}$ are linearly independent?

**Solution:** The set $\{a_1, a_2, a_3\}$ is linearly independent if $\lambda_1 a_1 + \lambda_2 a_2 + \lambda_3 a_3 = 0$ implies each of the $\lambda_i = 0$ for $i = 1, 2, 3$.

That is, $\lambda_1(4, 2, 1) + \lambda_2(2, -6, -5) + \lambda_3(1, -2, 3) = 0$

This yields the following system of homogeneous equations

$$4\lambda_1 + 2\lambda_2 + \lambda_3 = 0$$

$$2\lambda_1 - 6\lambda_2 - 2\lambda_3 = 0$$

$$\lambda_1 - 5\lambda_2 + 3\lambda_3 = 0$$

The above system will have trivial solution $\lambda_1 = \lambda_2 = \lambda_3 = 0$ if and only if $|A| \neq 0$, where $A$ is the coefficient matrix $\begin{bmatrix} 4 & 2 & 1 \\ 2 & -6 & -2 \\ 1 & -5 & 3 \end{bmatrix}$

We observe that $|A| = \begin{vmatrix} 4 & 2 & 1 \\ 2 & -6 & -2 \\ 1 & -5 & 3 \end{vmatrix} = -132 \neq 0$. Hence $\lambda_1 = \lambda_2 = \lambda_3 = 0$.

Thus the given vectors are linearly independent.

**Note:**

1. A set of vectors are linearly independent if $|A| \neq 0$ where $A$ is the matrix formed from the given vectors.
2. Maximum number of linearly independent vectors in $E^n$ is $n$. Hence any set of $n+1$ vectors are always linearly dependent.

**Problem**

Verify whether or not, the following set of vectors is linearly independent?

$$\{(4, 2, -1), (3, -6, -5)\}$$

**Ans.** The vectors are linearly independent.

**Problem** Verify whether or not, the following set of vectors is linearly independent?

$$\{(1, 1, 1), (0, 2, 3), (1, -2, 3)\}$$

**Ans:** The set of vectors is linearly independent.

**Problem 5** Verify whether or not, the following set of vectors is linearly independent?

$$\{(1, 2, 3), (1, 1, 1), (1, 0, 1)\}$$

$$\in L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}).$$

Therefore, $L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}) = L(S) = V$, which is a contradiction to the fact that $n$ is minimum with $S$ spans $V$. Therefore $S$ is linearly independent.

**Problem:** Define a maximal linearly independent set. Prove that a maximal linearly independent set is a basis.

**Solution:**

*Maximal linearly independent set:* A subset $S$ of a vector space $V$ is said to be a *maximal linearly independent set* if (i) $S$ is a linearly independent set, and (ii) $S \cup \{v\}$ is linearly dependent for any $v \in V \setminus S$.

Let $S = \{v_1, v_2, \dots, v_n\}$ be a maximal linearly independent set. In order to prove $S$ is a basis, it suffices to prove $S$ spans $V$.

Take $v \in V$. Suppose $\alpha_1 v_1 + \alpha_2 v_2 + \dots + \alpha_n v_n + \alpha v = 0$.

If $\alpha = 0$, then since $v_1, v_2, \dots, v_n$ are linearly independent, we get $\alpha_i = 0$ for all $1 \le i \le n$.

This means $v, v_1, v_2, \dots, v_n$ are (which are $n + 1$, in number) linearly independent, a contradiction to the maximality of $n$.

Therefore, $\alpha \neq 0$. Now $\alpha v = (-\alpha_1 v_1) + (-\alpha_2 v_2) + \dots + (-\alpha_n v_n)$.

This implies $v = (-\alpha_1 \alpha^{-1}) v_1 + (-\alpha_2 \alpha^{-1}) v_2 + \dots + (\alpha_n \alpha^{-1}) v_n$.

Therefore $S$ spans $V$. Hence $S$ is a basis.

**Problem 2:** Whether the vectors $\{a_1 = (4, 2, 1), a_2 = (2, -6, -5), a_3 = (1, -2, 3)\}$ are linearly independent?

**Solution:** The set $\{a_1, a_2, a_3\}$ is linearly independent if $\lambda_1 a_1 + \lambda_2 a_2 + \lambda_3 a_3 = 0$ implies each of the $\lambda_i = 0$ for $i = 1, 2, 3$.

That is, $\lambda_1 (4, 2, 1) + \lambda_2 (2, -6, -5) + \lambda_3 (1, -2, 3) = 0$

This yields the following system of homogeneous equations

$$4\lambda_1 + 2\lambda_2 + \lambda_3 = 0$$
$$2\lambda_1 - 6\lambda_2 - 2\lambda_3 = 0$$
$$\lambda_1 - 5\lambda_2 + 3\lambda_3 = 0$$

The above system will have trivial solution $\lambda_1 = \lambda_2 = \lambda_3 = 0$ if and only if $|A| \neq 0$, where $A$ is the coefficient matrix $\begin{bmatrix} 4 & 2 & 1 \\ 2 & -6 & -2 \\ 1 & -5 & 3 \end{bmatrix}$

We observe that $|A| = \begin{vmatrix} 4 & 2 & 1 \\ 2 & -6 & -2 \\ 1 & -5 & 3 \end{vmatrix} = -132 \neq 0$. Hence $\lambda_1 = \lambda_2 = \lambda_3 = 0$.

Thus the given vectors are linearly independent.

**Note:**

1. A set of vectors are linearly independent if $|A| \neq 0$ where $A$ is the matrix formed from the given vectors.
2. Maximum number of linearly independent vectors in $E^n$ is $n$. Hence any set of $n+1$ vectors are always linearly dependent.

**Problem**

Verify whether or not, the following set of vectors is linearly independent?

$$\{(4, 2, -1), (3, -6, -5)\}$$

**Ans.** The vectors are linearly independent.

**Problem** Verify whether or not, the following set of vectors is linearly independent?

$$\{(1, 1, 1), (0, 2, 3), (1, -2, 3)\}$$

**Ans:** The set of vectors is linearly independent.

**Problem 5** Verify whether or not, the following set of vectors is linearly independent?

$$\{(1, 2, 3), (1, 1, 1), (1, 0, 1)\}$$

**Ans:** linearly independent.

**Problem 6** Verify whether or not, the following set of vectors is linearly independent?

$$\{(1, 3, -2), (2, -1, 4), (1, -11, 14)\}$$

**Ans:** The set is not linearly independent

**Problem:** Show that if a set of vectors are linearly independent then every subset is also linearly independent.

**Solution:** Suppose that set of vectors $\{a_1, a_2, \dots, a_r\}$ are linearly independent.

Then $\lambda_1 a_1 + \lambda_2 a_2 + \dots + \lambda_r a_r = 0$ implies that all $\lambda_i$ are zero.

Consider the subset $\{a_1, a_2, a_3\}$. If these vectors are linearly dependent then $\lambda_1 a_1 + \lambda_2 a_2 + \lambda_3 a_3 = 0$ implies there exists say $\lambda_1 \neq 0$. But this contradicts that $\{a_1, a_2, \dots, a_r\}$ are linearly independent. The proof is complete.

**Exercises:**

1. Test whether or not the following set of vectors is linearly independent?
   i) $\{(2, 2, 3), (-1, -2, 1), (0, 1, 0)\}$
   ii) $\{(4, 2, 1), (2, -6, -5)\}$
   iii) $\{(4, 2, 1), (2, -6, -5), (1, -2, 3), (1, -1, 2)\}$

2. Show that if a set of vectors are linearly dependent then every superset is also linearly dependent.

3. Which of the following set of vectors forms a basis for $E^3$? Express $(3, 1, 2)$ as linear combination of basis vectors.
   i) $\{(2, 2, 3), (-1, -2, 1), (0, 1, 0)\}$
   ii) $\{(4, 2, 1), (2, -6, -5)\}$
   iii) $\{(4, 2, 1), (2, -6, -5), (1, -2, 3), (1, -1, 2)\}$

**Exercises**

1. Prove that the set $A = \{(2, -1, 0), (3, 5, 1), (1, 1, 2)\}$ forms a basis for $\mathbb{R}^3$ and express $(2, 4, 5)$ in terms of elements of $A$.

2. Check whether the following set of vectors form a basis for $\mathbb{R}^3$.
   (i) $B = \{(2, 1, 4), (1, -1, 2), (3, 1, -2)\}$
   (ii) $C = \{(1, 2, 1), (2, 1, 0), (1, -1, 2)\}$

3. Let $S = \{v_i \mid 1 \le i \le n\}$ is a subset of vector space $V$. If $v_j$ linear combination of its preceding ones, then prove that $L(\{v_1, v_2, \dots, v_{j-1}, v_{j+1}, \dots, v_n\}) = L(S)$.

4. Prove that for a vector space $V$ over a field $K$, if $v_i \in V, 1 \le i \le n$, then either they are linearly independent or some $v_k$ is a linear combination of the preceding ones $v_1, v_2, \dots, v_{k-1}$.