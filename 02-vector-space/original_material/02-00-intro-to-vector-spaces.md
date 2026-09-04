## 5. Vector Spaces and Inner-product spaces

### 5.1 Introduction

A **set** is a well-defined collection of objects in which we can say whether a given object is in the collection. The fact that $a$ is a member of a set $A$ is denoted by $a \in A$ and we call it as '$a$ belongs to $A$'. The members of a set are called **elements**.

A set is usually specified either by listing all of its elements inside a pair of braces or by stating the property that determines whether or not an object $x$ belongs to the set. We might write $S = \{x_1, x_2, \dots, x_n\}$.

**Example:** If $E$ is the set of even positive integers, we describe $E$ by writing either $E = \{2, 4, 6, \dots\}$
Or $E = \{x \mid x \text{ is an even integer and } x > 0\}$.
We write $2 \in E$ when we want to say that $2$ is in the set $E$, and $-3 \notin E$ to say that $-3$ is not in the set $E$.

**Notations:** Some of the more important set notations are given below:
$\mathbb{N}$: The set of all natural numbers $= \{n \mid n \text{ is a natural number}\} = \{1, 2, 3, \dots\}$;
$\mathbb{Z}$: The set of all integers $= \{x \mid x \text{ is an integer}\} = \{\dots, -1, 0, 1, 2, \dots\}$;
$\mathbb{Q}$: The set of all rational numbers $= \{p/q \mid p, q \in \mathbb{Z} \text{ where } q \neq 0\}$;
$\mathbb{R}$: The set of all real numbers $= \{x \mid x \text{ is a real number}\}$;
$\mathbb{C}$: The set of all complex numbers $= \{z \mid z \text{ is a complex number}\}$.

**Definitions:** If $x$ is not an element of $A$ then we write $x \notin A$. Suppose $A$ and $B$ are two sets. We say that $A$ is a **subset** of $B$ (written as $A \subseteq B$) if every element of $A$ is also an element of $B$. Two sets $A$ and $B$ are said to be **equal** (denoted by $A = B$) if $A$ is a subset of $B$, and $B$ is a subset of $A$. A set $B$ is a proper subset of $A$ if $B \subset A$ (that is, $B$ is a subset of $A$, but not equal to $A$). Trivially, every set is a subset of it self. A set which contains no elements at all is called the **Null set** (denoted by $\phi$).

For example, $\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$.

**Example:** Consider the sets $A = \{x \mid x \text{ is an even positive integer}\}$ and $B = \{x \mid x \text{ is a positive integer}\}$. Then $A \subseteq B$.

---

Operations on Sets:

(i) If $A$ and $B$ are two sets, then the set $\{x \mid x \in A \text{ or } x \in B\}$ is denoted by $A \cup B$ and we call it as the **union** of $A$ and $B$.

(ii) The set $\{x \mid x \in A \text{ and } x \in B\}$ is denoted by $A \cap B$ and we call it as the **intersection** of $A$ and $B$.

(iii) If $A$ and $B$ are two sets, then the set $\{x \in B \mid x \notin A\}$ is denoted by $B - A$ (or $B \setminus A$) and it is called as the **complement** $A$ in $B$.

(iv) The set that contains no members is called the **empty set** and it is denoted by $\phi$. Empty set is a subset of every set.

**Example:** Let $\mathbb{R}$ be the universal set and suppose that $A = \{x \in \mathbb{R} \mid 0 < x \le 3\}$ and $B = \{x \in \mathbb{R} \mid 2 \le x < 4\}$. Then
$A \cap B = \{x \in \mathbb{R} \mid 2 \le x \le 3\}$;
$A \cup B = \{x \in \mathbb{R} \mid 0 < x < 4\}$;
$A \setminus B = \{x \in \mathbb{R} \mid 0 < x < 2\}$;
$A' = \{x \in \mathbb{R} \mid x \le 0 \text{ or } x > 3\}$.

**Note:** The operations of union and intersection can be defined for three or more sets in the similar way.
$A \cup B \cup C = \{x \mid x \in A \text{ or } x \in B \text{ or } x \in C\}$ and
$A \cap B \cap C = \{x \mid x \in A, x \in B, x \in C\}$

---

**Note:** The operations of union and intersection can be defined for three or more sets in the similar way.
$A \cup B \cup C = \{x \mid x \in A \text{ or } x \in B \text{ or } x \in C\}$ and
$A \cap B \cap C = \{x \mid x \in A, x \in B, x \in C\}$

In general, let $A_i$ be a collection of sets – one for each element $i$ belongs to $I$, where $I$ is some set ($I$ may be the set of all positive integers). We define
$\displaystyle\bigcap_{i \in I} A_i = \{a \mid a \in A_i \text{ for all } i \in I\}$, and
$\displaystyle\bigcup_{i \in I} A_i = \{a \mid a \in A_i \text{ for some } i \in I\}$.

A collection $\{A_i\}_{i \in I}$ of sets is said to be *mutually disjoint* if $A_i \cap A_j = \phi$ for all $i \in I$, $j \in I$ such that $i \neq j$.

**Example:**
(i) Write $A_i = \{i, i+1, i+2, \dots\}$ for each $i \in N$, the set of natural numbers. Then it is easy to observe that $\displaystyle\bigcup_{i \in N} A_i = N$ and $\displaystyle\bigcap_{i \in I} A_i = \Phi$.

(ii) If $B_i = \{2i, 2i+1\}$ for all $i \in N$, then $\{B_i\}_{i \in N}$ is a collection of mutually disjoint sets.

**Definition:** Let $A$ and $B$ are two sets. We define their symmetric difference as the set $A \Delta B = (A-B) \cup (B-A)$. Sometimes it is denoted by $A \oplus B$.

**Example:** If $A = \{1, 2, 3, 4\}$ and $B = \{1, 2, 5, 7\}$, then $A \oplus B = \{3, 4, 5, 7\}$.

The set operations satisfy the following properties.
1. $A \cup B = B \cup A$; $A \cap B = B \cap A$ (commutative properties)
2. $A \cup (B \cup C) = (A \cup B) \cup C$; $A \cap (B \cap C) = (A \cap B) \cap C$ (Associative)
3. $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$; $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$ (Distributive)
4. $A \cup A = A$; $A \cap A = A$ (Idempotent)
5. $(A')' = A$
6. $A \cup A' = \cup$
7. $A \cap A' = \phi$
8. $\phi' = \cup$
9. $\cup' = \phi$
10. $(A \cup B)' = A' \cap B'$; $(A \cap B)' = A' \cup B'$ (D' Morgan laws)
11. $A \cup \phi = A$; $A \cap \phi = \phi$; $A \cup \cup = \cup$; $A \cap \cup = A$ (Universal)

**Note:** Let $|A|$ denote the number of elements in the set $A$.
For any two sets $P$ and $Q$, we have
(i). $|P \cup Q| \le |P| + |Q|$ (ii). $|P \cap Q| \le \min (|P|, |Q|)$
(iii). $|P \oplus Q| = |P| + |Q| - 2|P \cap Q|$ where $\oplus$ is the symmetric difference.

**Definition:** (i) If $S$ and $T$ are two sets, then the set $\{(s, t) / s \in S \text{ and } t \in T\}$ is called the **Cartesian product** of $S$ and $T$
(here $(a, b) = (s, t) \iff a = s \text{ and } b = t$). The Cartesian product of $S$ and $T$ is denoted by $S \times T$.
Thus $S \times T = \{(s, t) / s \in S \text{ and } t \in T\}$.
Note that if $S$ and $T$ are two sets, then $S \times T$ and $T \times S$ may not be equal.
(ii) If $S_1, S_2, \dots, S_n$ are $n$ sets, then the **Cartesian product** is defined as
$S_1 \times S_2 \times \dots \times S_n = \{(s_1, s_2, \dots, s_n) / s_i \in S_i \text{ for } 1 \le i \le n\}$.
Here the elements of $S_1 \times S_2 \times \dots \times S_n$ are called **ordered n-tuples**. For any two n-tuples, we have $(s_1, s_2, \dots, s_n) = (t_1, t_2, \dots, t_n) \iff s_i = t_i, 1 \le i \le n$.

**Example:** If $X = \{a, b\}$ and $Y = \{x, y\}$, then
$X \times Y = \{(a, x), (a, y), (b, x), (b, y)\}$ and $Y \times X = \{(x, a), (x, b), (y, a), (y, b)\}$.
Note that $X \times Y \neq Y \times X$.

**Definition:** Let $S$ and $T$ be sets. A **function** $f$ from $S$ to $T$ is a subset $f$ of $S \times T$ such that

---

(i) for $s \in S$, there exists $t \in T$ with $(s, t) \in f$,

(ii) $(s, u) \in f$ and $(s, t) \in f \implies t = u$.

If $(s, t) \in f$, then we write $(s, f(s))$ or $f(s) = t$.

Here $t$ is called the **image** of $s$; and $s$ is called the **preimage** of $t$.

The set $S$ is called the **domain** of $f$ and $T$ is called the **codomain**.

The set $\{f(s) / s \in S\}$ is a subset of $T$ and it is called the **image** of $S$ under $f$ (or image of $f$). We denote the fact: '$f$ is a function from $S$ to $T$' by "$f: S \to T$".

**Example:** Let $\mathbb{R}$ be the set of real numbers. Define $f(x) = x^2$ for every $x \in \mathbb{R}$. This represents a function $f = \{(x, x^2) \mid x \in \mathbb{R}\}$.

**Example:** Let $f: \mathbb{N} \to \mathbb{N}$ be a function such that $f(x) = x \pmod 3$. That is $f(x)$ is the remainder obtained when $x$ is divided by 3. Then the domain of $f$ is $\mathbb{N}$ and the range of $f$ is $\{0, 1, 2\}$.

**Definition:** $f: S \to T$ is said to be

(i) **one-one function** (or **injective function**) if it satisfies the following condition: $f(s_1) = f(s_2) \implies s_1 = s_2$.

(ii) **onto function** (or **surjective function**) if it satisfies the following condition: $t \in T \implies \text{there corresponds an element } s \text{ in } S \text{ such that } f(s) = t$.

(iii) a **bijection** if it is both one-one and onto.

**Definition:** Let $g: S \to T$ and $f: T \to U$. The **composition** of $f$ and $g$ is a function $f \circ g: S \to U$ defined by $(f \circ g)(s) = f(g(s))$ for all $s$ in $S$.

That is, $f \circ g = \{(s, u) \mid s \in S, u \in U \text{ and } \exists\, t \in T \text{ and } t = g(s) \text{ and } u = f(t)\}$.
**Example:** Let $f: \mathbb{R} \to \mathbb{R}$ and $g: \mathbb{R} \to \mathbb{R}$ where $\mathbb{R}$ is the set of real numbers. If $f(x) = x^2 - 2$ and $g(x) = x + 4$. Find $g \circ f$ and $f \circ g$

Solution: $(g \circ f)(x) = g(f(x)) = g(x^2 - 2) = (x^2 - 2) + 4 = x^2 + 2$; and

$(f \circ g)(x) = f(g(x)) = f(x + 4) = (x + 4)^2 - 2 = x^2 + 8x + 14$.

