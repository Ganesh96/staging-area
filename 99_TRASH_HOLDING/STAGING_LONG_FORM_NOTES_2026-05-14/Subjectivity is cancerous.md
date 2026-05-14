I will give you a clean, fully formal mathematical version.

We will prove two things:

1. If tastes are “subjective” but monotone in some shared parameters, then Pareto-dominance ⇒ universal agreement that one work is better.
    
2. Under mild assumptions (compactness) there must exist undominated (“objectively great”) works.
    

---

## 1. Formal setup

### 1.1 Sets and parameters

Let

- (A) be a nonempty set of “works” (movies, books, etc.).
    
- (n \in \mathbb{N}) be the number of parameters.
    

Define a function  
[  
f : A \to \mathbb{R}^n,  
]  
where for (a \in A),  
[  
f(a) = (f_1(a), f_2(a), \dots, f_n(a)).  
]

Each (f_i : A \to \mathbb{R}) is the (i)-th parameter (e.g. acting, structure, etc.).

We impose a coordinatewise partial order on (\mathbb{R}^n):

For (x = (x_1,\dots,x_n), y = (y_1,\dots,y_n) \in \mathbb{R}^n), define:

- (x \ge y) iff (x_i \ge y_i) for all (i = 1,\dots,n).
    
- (x > y) iff (x \ge y) and there exists (j) such that (x_j > y_j).
    

We assume:

**Assumption (shared direction of improvement).**  
For each coordinate (i), “larger” means “no worse.”

This is encoded in the monotonicity we give to preferences below.

---

### 1.2 Agents and tastes

Let (K) be a (possibly infinite) index set of agents.

Each agent (k \in K) has a utility function  
[  
U_k : A \to \mathbb{R}  
]  
defined by  
[  
U_k(a) = g_k(f(a)) = g_k(f_1(a), \dots, f_n(a)),  
]  
for some function (g_k : \mathbb{R}^n \to \mathbb{R}).

We assume:

**Assumption (strict coordinatewise monotonicity).**  
For each (k \in K), for all (x, y \in \mathbb{R}^n),  
[  
\Big( x \ge y \text{ and } x \neq y \Big) ;\Rightarrow; g_k(x) > g_k(y).  
]  
Equivalently: if every coordinate is at least as large and at least one strictly larger, the utility strictly increases.

This is the only “rationality” assumption. Tastes are “subjective” because the (g_k) can be arbitrarily different across (k).

Define the preference relation for each agent (k) by:  
[  
a \succeq_k b ;\Longleftrightarrow; U_k(a) \ge U_k(b),  
]  
[  
a \succ_k b ;\Longleftrightarrow; U_k(a) > U_k(b).  
]

---

### 1.3 Pareto dominance on works

We define a **Pareto dominance** relation on (A):

For (a,b \in A),

- (a \succeq_P b) (“Pareto weakly dominates”) iff  
    [  
    f(a) \ge f(b),  
    ]  
    i.e. (f_i(a) \ge f_i(b)) for all (i).
    
- (a \succ_P b) (“Pareto strictly dominates”) iff  
    [  
    f(a) \ge f(b) \text{ and } f(a) \neq f(b),  
    ]  
    i.e. (f_i(a) \ge f_i(b)) for all (i) and (f_j(a) > f_j(b)) for some (j).
    

---

## 2. The key theorem: Pareto dominance ⇒ universal preference

### Theorem 1

For any (a,b \in A),

[  
a \succ_P b ;\Longrightarrow; \forall k \in K,; a \succ_k b.  
]

In words: if (a) Pareto-dominates (b), then every agent strictly prefers (a) over (b).

#### Proof

Fix arbitrary (a,b \in A) such that (a \succ_P b).

By definition of (\succ_P):

1. (f(a) \ge f(b)):  
    [  
    \forall i \in {1,\dots,n},; f_i(a) \ge f_i(b).  
    ]
    
2. (f(a) \neq f(b)):  
    Hence there exists some (j \in {1,\dots,n}) with  
    [  
    f_j(a) > f_j(b).  
    ]
    

Define  
[  
x := f(a) = (f_1(a),\dots,f_n(a)), \quad  
y := f(b) = (f_1(b),\dots,f_n(b)).  
]

Then:

- (x \ge y),
    
- (x \neq y).
    

Now fix arbitrary (k \in K).

By Assumption (strict coordinatewise monotonicity) for (g_k):

[  
x \ge y \text{ and } x \neq y ;\Rightarrow; g_k(x) > g_k(y).  
]

Substitute:  
[  
g_k(x) = g_k(f(a)) = U_k(a), \quad  
g_k(y) = g_k(f(b)) = U_k(b).  
]

Thus we obtain:  
[  
U_k(a) > U_k(b).  
]

But this is exactly (a \succ_k b) by definition of (\succ_k).

Since (k \in K) was arbitrary, we have:  
[  
\forall k \in K,; a \succ_k b.  
]

This completes the proof. (\square)

---

Interpretation (in pure math terms):

> The relation (\succ_P) is a refinement of all strictly monotone utility-induced preference relations ( \succ_k ).  
> Any pair ordered by (\succ_P) is ordered the same way by every such (\succ_k).

This is already a **precise, fully formal sense** in which “X is better than Y even though taste is subjective.”

---

## 3. Existence of “objectively great” (undominated) works

Now we prove that under standard topological assumptions, there must exist Pareto-undominated elements of (A).

These will be the candidates for “objectively great” works: nothing is strictly better in all coordinates.

### 3.1 Image set and compactness

Let  
[  
S := f(A) \subseteq \mathbb{R}^n  
]  
be the set of all parameter vectors of works.

Assume:

**Assumption (compactness).**  
(S) is a nonempty compact subset of (\mathbb{R}^n).

This is a standard assumption in analysis/optimization: bounded and closed; for example if parameters are normalized to a closed, bounded region.

We will show:

> There exists (x^* \in S) that is Pareto-maximal in (S):  
> no (y \in S) with (y \ge x^_) and (y \neq x^_).

Then the associated work (a^* \in A) with (f(a^_) = x^_) is “objectively great” in the sense of being undominated.

---

### 3.2 Existence of Pareto-maximal point in a compact set

Define the function  
[  
h : \mathbb{R}^n \to \mathbb{R}, \quad  
h(x_1,\dots,x_n) = x_1 + x_2 + \dots + x_n.  
]

Observe:

- (h) is continuous.
    
- Therefore, by the extreme value theorem, since (S) is compact and nonempty, there exists some (x^* \in S) such that  
    [  
    h(x^*) = \max_{x \in S} h(x).  
    ]
    

We claim that this (x^*) is Pareto-maximal in (S).

#### Claim

There is no (y \in S) with (y \ge x^_) and (y \neq x^_).

#### Proof of claim

Suppose, for contradiction, that there exists (y \in S) such that:

1. (y \ge x^_), i.e. (\forall i,; y_i \ge x^__i).
    
2. (y \neq x^_), so (\exists j) with (y_j > x^__j).
    

Compute:  
[  
h(y) = \sum_{i=1}^n y_i.  
]

Since (y_i \ge x^__i) for all (i), we have  
[  
h(y) \ge \sum_{i=1}^n x^__i = h(x^*).  
]

Because there is at least one strict inequality (y_j > x^__j), it follows that  
[  
h(y) > h(x^_).  
]

But this contradicts the maximality of (h(x^*)) on (S).

Therefore, no such (y) can exist and (x^*) is Pareto-maximal in (S). (\square)

---

### 3.3 Lifting back to works

Since (x^* \in S = f(A)), there exists at least one (a^* \in A) such that  
[  
f(a^_) = x^_.  
]

We have just proved:

> For all (b \in A), it is not the case that (f(b) \ge f(a^_)) with (f(b) \neq f(a^_)).

Equivalently:

[  
\forall b \in A,; \neg ( b \succ_P a^* ).  
]

So (a^*) is **not Pareto-dominated by any other work**.

This is a purely mathematical existence theorem: given compactness of the parameter image set, there must exist such an undominated work.

We may call such an (a^*) “objectively great” in the sense:

- There is no other work that is at least as good in every parameter and strictly better in at least one.
    

---

## 4. Stronger notion: universally best work (if it exists)

The previous step guarantees undominated works, not necessarily a single “best of all” that dominates everything.

However, if there happens to exist some point that dominates everything, we can prove universal best-ness.

### Definition

A work (a^\dagger \in A) is **globally Pareto-superior** if:

[  
\forall b \in A,; f(a^\dagger) \ge f(b).  
]  
and for each (b \neq a^\dagger), there exists at least one coordinate (j) with  
[  
f_j(a^\dagger) > f_j(b).  
]

This is stronger than Pareto-maximal: (a^\dagger) dominates everything.

### Theorem 2

If such an (a^\dagger) exists, then for every agent (k \in K) and every work (b \in A) with (b \ne a^\dagger),  
[  
a^\dagger \succ_k b.  
]

So (a^\dagger) is strictly preferred by all agents to all other works.

#### Proof

Fix arbitrary (k \in K) and (b \in A) with (b \neq a^\dagger).

By global Pareto-superiority, we have:

- (f(a^\dagger) \ge f(b)),
    
- (f(a^\dagger) \neq f(b)).
    

Define  
[  
x = f(a^\dagger),\quad y = f(b).  
]

Then (x \ge y) and (x \neq y).

By strict monotonicity of (g_k),  
[  
g_k(x) > g_k(y).  
]

Therefore,  
[  
U_k(a^\dagger) = g_k(f(a^\dagger)) = g_k(x) > g_k(y) = g_k(f(b)) = U_k(b),  
]  
i.e.  
[  
a^\dagger \succ_k b.  
]

Since (k) and (b) were arbitrary, the result holds for all agents and all other works. (\square)

This is the exact formalization of:

> If some work is at least as good on every parameter and strictly better on at least one, compared to every other work, then all agents (with monotone tastes) must rank it as the best.

---

## 5. Summary in pure math

1. We model works as points in (\mathbb{R}^n) via (f : A \to \mathbb{R}^n).
    
2. We model subjective tastes as arbitrary strictly coordinatewise-increasing functions (g_k : \mathbb{R}^n \to \mathbb{R}).
    
3. We define Pareto dominance via the product order on (\mathbb{R}^n).
    
4. We proved:
    
    - **Theorem 1:**  
        [  
        a \succ_P b \Rightarrow \forall k,; a \succ_k b.  
        ]  
        Pareto dominance implies universal strict preference.
        
    - **Existence result (via compactness):**  
        If (S = f(A)) is compact, then there exists (x^_) Pareto-maximal in (S), hence at least one undominated work (a^_).
        
    - **Theorem 2 (strong case, if it happens):**  
        If (a^\dagger) dominates all others (coordinatewise), then (a^\dagger) is strictly preferred by every agent to every other work.
        

Mathematically, this is a rigorous, step-by-step proof that:

- Even with fully subjective utility functions (one per agent),
    
- As long as they are strictly monotone in some shared parameters,
    
- There is a clear sense in which some works are **objectively better** (Pareto-dominant) and some works are **objectively great** (Pareto-undominated), and in the strong case, universally best.