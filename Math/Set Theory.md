**Set theory** is the branch of mathematical logic that studies sets, which can be informally described as collections of objects. Although objects of any kind can be collected into a set, set theory, as a branch of mathematics, is mostly concerned with those that relevant to mathematics as a whole


### 1. Introduction

- A **set** is a collection of objects called **elements**

**List notation examples:**
$A = \{x\ |\ x \in N\} \Rightarrow A = \{1,\ 2,\ 3,\ 4,\ \dots\}$ 
$B = \{x\ |\ x \in Z\} \Rightarrow B = \{-3,-2,-1,0,\ \dots\}$

* **Sets** can be *finite* or *infinite*:
$A = \{1,\ 2, \ 3,\ 4,\ 5,\ 6,\ 7,\ 8\}$ - Finite set
$Z^+ = \{1,\ 2, \ 3,\ 4,\ \dots \}$ - Implied pattern forever

**Common sets**:
* Natural Numbers $N = \{1,\ 2, \ 3,\ 4,\ \dots \}$
* Integers $Z = \{-2,-1, \ 0,\ 1,\ 2,\ \dots \}$
* Rational Numbers $Q = \{-\frac{3}{2},-\frac{1}{2}, \ \frac{4}{3},\ \frac{5}{3},\ \dots \}$

**Elements and cardinality:**
* $Let\ C = \{11,\ 12,\ 13\}$
* Eleven **is an element** of C: $11 \in C$
* Two **is not an element** of C: $2 \notin C$
* The **cardinality (size)** of C is 3: $|C| = 3$ or #$C=3$

**Empty set:**
* $\varnothing = \{\}$
* $|\varnothing| = 0$
* $|\{\varnothing\}| = 1$ (because we have one element in set)

**Self-Builder Notation:**
* $Q = \{\frac{m}{n}\ |\ m,n \in Z,\ n \neq 0\}$
* $2Z = \{\dots,-4,-2,\ 0,\ 2,\ \dots \} = \{2n\ |\ n \in Z \}$


### 2. Cartesian Product and ordered pairs

* An ordered pair $(a, b)$ is a set $\{\{a\},\ \{a,b\}\}$

**Cartesian Product, $A \times B$**, is the set
* $A \times B = \{(a,\ b)\ |\ a \in A\ and\ b \in B\}$

$Given\ X = \{0,1,2\}\ and\ Y = \{0, 1\}$
$X \times Y = \{(0,0),\ (0,1),\ (1,0),\ (1,1),\ (2,0),\ (2,1)\}$
$Y \times X = \{(0,0),\ (1,1),\ (0,2),\ (1,0),\ (0,1),\ (1,2)\}$

**Cardinality of $A \times B$**:
* $|A \times B| = |A| \times |B|$

**Cartesian Products can generalise to n-tuples:**
* 3-tuple: $A \times B \times C = \{(a,b,c)\ |\ a \in A,\ b \in B,\ c \in C\}$
* n-tuple: $A_1 \times A_2 \times \dots \times A_n = \{(a_1,a_2,\dots,a_n)\ |\ a_1 \in A_1,\ a_2 \in A_2, \dots, a_n \in A_n\}$

$Let\ B = \{c,\ d\}$
$B^2 = B \times B = \{(c,c),\ (c,d),\ (d,c),\ (d,d)\}$
$\varnothing \times B = \varnothing$


### 3. Subsets and power sets

* If **A** is a **subset** of **B**, then every element in A must also be in B ($A \subseteq B$)

Examples:
* $\{a,\ b\} \subseteq \{a,\ b,\ c\}$ (All elements in the set)
* $\{c,\ d\} \subseteq \{c,\ d\}$
* $\{a\} \not\subseteq \{\{a\}\}$ (The set has no element $a$)
* $\varnothing \subseteq \{x,\ y,\ z\}$ (Empty-set is included in any set)

A **power set of A**, $p(A)$, is the set containing all possible subsets of A
* $A = \{a,\ b\},\ p(A) = \{\varnothing,\ \{a\},\ \{b\},\ \{a,\ b\}\}$

If $|A|$ = n, then $|p(A)| = 2^{|A|} = 2^n$

* $p(\varnothing) = 2^0 = 1$
* $p(\{\varnothing\}) = 2^1 = 2$
* $A \not\subseteq p(A)$, but $A \in p(A)$

If $|C| = k$ and $|D| = j$, then $|p(C \times D)| = 2^{|C|*|D|} = 2^{kj}$


### 4. Set operations

The **complement** of A is written as $\bar A$
* $\bar A = \{a \in U\ |\ a \not\in A\}$

The **intersection** of A and B is
* $A \cap B = \{x\ |\ x \in A\ and\ x \in B\}$

The **union** of A and B is
* $A \cup B = \{x\ |\ x \in A\ or\ x \in B\}$

The **difference**, A-B, is defined as
* $A - B = \{x\ |\ x \in A\ and\ x \not\in B\}$

The **symmetric difference** (xor), $A \oplus B$ (or $A\ \triangle\ B$), is defined as
* $A\ \triangle\ B = (A-B) \cup (B-A)$