
### {1} Définitions et exemples 

> [!Def]+ Définition : anneau
> - Un **anneau** est un ensemble $A$ muni de deux lois de composition internes
>   $$ +: A \times A \rightarrow A \quad (x,y) \mapsto x + y $$
>   $$ \cdot : A \times A \rightarrow A \quad (x,y) \mapsto x \cdot y $$
>   telles que
>   
>    1. $(A, +)$ est un groupe abélien,
>    2. la loi $\cdot$ est associative $(x \cdot (y \cdot z) = (x \cdot y) \cdot z$ pour tous $x,y,z \in A)$,
>    3. il existe un neutre pour la loi $\cdot$,
>    4. distributivité : 
>    $$ x \cdot (y + z) = x \cdot y + x \cdot z $$
>    $$ (x + y) \cdot z = x \cdot z + y \cdot z $$
> pour tous $x,y,z \in A$.
> 
> Si de plus la loi $\cdot$ est commutative on dit que $A = (A, +, \cdot)$ est un **anneau commutatif**.

^fb6a8d


> [!Lem]+ Lemme 2.3
> - Soit $A$ un anneau. 
> 
> ▷ Alors :
>    1. $0 \cdot x = 0 = x \cdot 0$ pour tout $x \in A$,
>    2. $(-x) \cdot y = -(x \cdot y) = x \cdot (-y)$ pour tous $x,y \in A$.

^e20071


> [!Def]+ Définition 2.4
> - Soit $A$ un anneau. 
> 
> ▷ Le sous-ensemble
>   $$ U(A) := \{u \in A | \exists v \in A \text{ tel que } uv = 1 = vu\} \subseteq A $$
>   est appelé **unités de $A$**.

^82b108

> [!Expl]+ Exemples d’*unité d’anneaux* : 
> $$U(\mathbb{Z})=\{ -1,1 \}$$
> $$U(\mathbb{Q})=\mathbb{Q}^{*}$$
> $$U(\mathbb{Z}/n\mathbb{Z})=(\mathbb{Z}/n\mathbb{Z})^{\times}$$
> $$U(M_{n}(\mathbb{R}))=GL(n,\mathbb{R})$$

^53262e


> [!Def]+ Déf d’un corps par un anneau
> - Un anneau $A$ est un **corps** si $A$ est commutatif et $U(A) = A \setminus \{0\}$.

^1f962b

> [!Def]+ Déf: diviseur de 0
> - Soit $A$ un anneau. 
> 
> ▷ Un élément $a \in A \setminus \{0\}$ est un **diviseur de 0** si il existe $0 \neq b \in A$ tel que
>   $$ ab = 0 \quad \text{ou} \quad ba = 0. $$

^89d91e

> [!Def]+ Déf : Anneau intègre
> - Un anneau *commutatif* $A \neq \{0\}$ est dit **intègre** s’il ne contient pas de diviseurs de 0.

^8857d6

> [!Prop]+ Proposition 2.10
> - Soit $A$ un *anneau fini*. 
>
> ▷ Alors $A$ est un corps *ssi* $A$ est intègre.

^30e32f

> [!Def]+ Déf : sous-anneau
> - Soit $A$ un anneau. 
> 
> ▷ Un sous-ensemble $B \subseteq A$ est un **sous-anneau** si 
>
>- l’addition et la multiplication de $A$ se restreignent à des lois internes sur $B$ tel que
>   $$(B, +, \cdot) \quad \text{est un anneau avec} \quad 1_B = 1_A. $$
> 
> > Pas besoin de demander pour $0_B$ comme il s’agit d’une conséquence du reste



^746671

### {2} Homomorphisme d’anneaux

> [!Def]+ Déf : homomorphisme d’anneaux
> - Soient $A, B$ deux anneaux. 
> 
> ▷ Une application $f : A \rightarrow B$ est un **homomorphisme d'anneaux** si
>   1. $f(x + y) = f(x) + f(y)$ pour tous $x, y \in A$
>   2. $f(1_A) = 1_B$
>   3. $f(x \cdot y) = f(x) \cdot f(y)$ pour tous $x, y \in A$.


^b8bd60

> [!Def]+ Déf: isomorphisme d’anneaux
> - Si il existe un homomorphisme d’anneaux $f' : B \rightarrow A$ tel que
>    $$ f' \circ f = \text{Id}_A \quad \text{et} \quad f \circ f' = \text{Id}_B $$
>    
> ▷ Alors $f$ est un **isomorphisme d'anneaux**. 
> Dans ce cas, on dit que $A$ et $B$ sont **isomorphes** et on le dénote par $A \cong B$.

^a64e7c


> [!Prop]+ Proposition 2.14
> - Un homomorphisme d’anneaux est un isomorphisme si et seulement si il est bijectif.

^5cf24d

> [!Lem]+ Lemme 2.15
> - Soit $f : A \rightarrow B$ un homomorphisme d’anneaux. 
> 
> ▷ Alors
>   1. $\text{Ker}(f)$ est un sous-groupe de $(A, +)$,
>   2. Pour tous $k \in \text{Ker}(f)$ et $a \in A$ on a $k \cdot a \in \text{Ker}(f)$ et $a \cdot k \in \text{Ker}(f)$.

^a7443c

> [!Lem]+ Lemme 2.16
> - Soient $A$ un anneau, $a \in A$ et $m \in \mathbb{Z}$. 
> 
> ▷ Alors
>   $$ (m \cdot 1_A) \cdot a = m \cdot a. $$

^c75a26


> [!Cor]+ Corollaire 2.17
> - Soit $A$ un anneau. 
> 
> ▷ Si il existe $m \in \mathbb{Z}$ tel que $m \cdot 1_A = 0_A$ 
> 
> ▷ alors,
> 	 $m \cdot a = 0_A$ pour tout $a \in A$.

^fe9401

^ceb743