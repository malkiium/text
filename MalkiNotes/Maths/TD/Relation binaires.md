[[relation binaire]]

#relationsbinaires #mathématiques #relationdéquivalence #relationdordre #réflexivité #symétrie #transitivité #grapheorienté #matricedadjacence

## Définition

Une **relation binaire** sur un ensemble $E$ est un sous-ensemble du produit cartésien $E\times E$. Autrement dit, une relation $R$ est un ensemble de couples $(x,y)$ où $x,y\in E$.

**Explication** : Une relation binaire associe chaque élément de l'ensemble $E$ avec un autre élément de cet ensemble, formant ainsi des paires ordonnées. Par exemple, une relation peut lier les éléments de l'ensemble $E$ comme dans le cas de l'égalité ou de l'infériorité.

## Notations

- $(x,y)\in R$ : "x est en relation avec y"
- $xRy$ : notation usuelle pour signifier que $(x,y)$ appartient à $R$

**Explication** : Cette notation signifie qu'il existe une relation entre $x$ et $y$. Par exemple, $xRy$ peut signifier que $x$ est inférieur ou égal à $y$ dans le cas d'une relation d'ordre.

## Propriétés des relations binaires

Une relation binaire peut posséder différentes propriétés :

### 1. Réflexivité

Une relation $R$ est **réflexive** si : $∀x∈E,(x,x)∈R$

**Explication** : Une relation est réflexive si chaque élément de l'ensemble est en relation avec lui-même. Par exemple, dans la relation d'égalité, chaque nombre est égal à lui-même : $x = x$.

### 2. Symétrie

Une relation $R$ est **symétrique** si : $∀x,y∈E,(x,y)∈R⇒(y,x)∈R$

**Explication** : Une relation est symétrique si, chaque fois qu'un élément $x$ est en relation avec un élément $y$, $y$ est aussi en relation avec $x$. Par exemple, dans la relation "être ami avec", si $x$ est ami avec $y$, alors $y$ est aussi ami avec $x$.

### 3. Antisymétrie

Une relation $R$ est **antisymétrique** si : $∀x,y∈E,(x,y)∈R \text{ et } (y,x)∈R ⇒ x=y$

**Explication** : Une relation est antisymétrique si, lorsque deux éléments sont en relation dans les deux sens (c'est-à-dire $(x,y) \in R$ et $(y,x) \in R$), alors ils doivent être égaux. Par exemple, dans la relation "être inférieur ou égal à" sur les réels, si $x \leq y$ et $y \leq x$, alors $x = y$.

### 4. Transitivité
 
Une relation $R$ est **transitive** si : $∀x,y,z∈E,(x,y)∈R \text{ et } (y,z)∈R⇒(x,z)∈R$

**Explication** : Une relation est transitive si, chaque fois que $x$ est en relation avec $y$ et que $y$ est en relation avec $z$, alors $x$ est aussi en relation avec $z$. Par exemple, dans la relation "être inférieur ou égal à", si $x \leq y$ et $y \leq z$, alors $x \leq z$.

## Types particuliers de relations

### 1. Relation d’équivalence

Une relation $R$ est une **relation d’équivalence** si elle est :

- Réflexive
- Symétrique
- Transitive

**Explication** : Une relation d'équivalence permet de diviser l'ensemble $E$ en sous-ensembles appelés **classes d'équivalence**. Par exemple, l'égalité sur les réels est une relation d'équivalence, car elle est réflexive, symétrique et transitive.

### 2. Relation d’ordre

Une relation $R$ est une **relation d’ordre** si elle est :

- Réflexive
- Antisymétrique
- Transitive

**Explication** : Une relation d'ordre impose une structure où les éléments sont comparables entre eux, souvent utilisée pour trier des objets. Si, en plus, chaque élément est comparable à un autre, la relation devient un **ordre total**. Sinon, c'est un **ordre partiel**. Par exemple, l'infériorité ou égalité ($\leq$) sur les réels est un ordre total.

## Représentation des relations binaires

### 1. Matrice d’adjacence

Une relation $R$ sur $E$ peut être représentée par une matrice $M$ où :

- $M_{ij}=1$ si $(x_i,x_j)\in R$
- $M_{ij}=0$ sinon

**Explication** : Cette matrice est une façon de représenter graphiquement les relations entre les éléments de $E$. Chaque case de la matrice indique si une relation existe entre deux éléments spécifiques de l'ensemble $E$.

### 2. Graphe orienté

Une relation peut aussi être représentée par un graphe où :

- Les éléments de $E$ sont les sommets
- Un arc orienté de $x$ vers $y$ existe si $(x,y)\in R$

**Explication** : Dans un graphe orienté, les éléments de $E$ sont représentés par des sommets, et les relations entre eux par des arcs dirigés. Cela permet de visualiser comment les éléments sont en relation les uns avec les autres.

## Exemples

1. **Égalité sur $\mathbb{Z}$** : $x=y$ est une relation d’équivalence.
    
    **Explication** : L'égalité est une relation qui satisfait la réflexivité (chaque nombre est égal à lui-même), la symétrie (si $x = y$, alors $y = x$) et la transitivité (si $x = y$ et $y = z$, alors $x = z$).
    
2. **Infériorité sur $\mathbb{N}$** : $x\leq y$ est une relation d’ordre total.
    
    **Explication** : L'infériorité ou égalité sur les entiers naturels est une relation d'ordre total, car tout élément de $\mathbb{N}$ est comparable à un autre.
    
3. **Divisibilité sur $\mathbb{N}$** : $x \mid y$ est une relation d’ordre partiel.
    
    **Explication** : La divisibilité sur $\mathbb{N}$ est une relation d'ordre partiel, car certains éléments ne sont pas comparables (par exemple, $6$ et $10$ ne sont ni divisibles l'un par l'autre).
    

## Opérations sur les relations

- **Intersection** : $R_1\cap R_2$
    
    **Explication** : L'intersection de deux relations consiste à prendre les éléments qui sont en relation dans les deux relations.
    
- **Union** : $R_1\cup R_2$
    
    **Explication** : L'union de deux relations consiste à combiner les relations des deux ensembles, en gardant tous les couples.
    
- **Composition** : $R_1\circ R_2$, où $(x,z)\in R_1\circ R_2$ si $\exists y, (x,y)\in R_1$ et $(y,z)\in R_2$
    
    **Explication** : La composition de deux relations consiste à relier un élément $x$ à un élément $z$ si et seulement si il existe un élément intermédiaire $y$ tel que $x$ soit en relation avec $y$ et $y$ soit en relation avec $z$.
    
- **Clôture transitive** : Plus petite relation transitive contenant $R$
    
    **Explication** : La clôture transitive d'une relation est la plus petite relation transitive qui contient cette relation. Elle permet d'ajouter les relations nécessaires pour que la transitivité soit satisfaite.

### Exemple : Relation d'égalité

Sur un ensemble $E$, définissons la relation $R$ comme suit :  
$R = {(x, y) \in E \times E \mid x = y}$.

Cela signifie que $x$ est en relation avec $y$ si et seulement si $x$ est égal à $y$. Analysons les propriétés :

- **Réflexivité** : Pour tous les éléments $x \in E$, $(x, x) \in R$ car $x = x$.
    
- **Symétrie** : Si $(x, y) \in R$, cela signifie que $x = y$. Par symétrie de l'égalité, $y = x$, donc $(y, x) \in R$.
    
- **Antisymétrie** : Si $(x, y) \in R$ et $(y, x) \in R$, cela signifie que $x = y$ et $y = x$. Par conséquent, $x = y$, ce qui satisfait la condition de l'antisymétrie.
    

Ainsi, la relation **d'égalité** est **réflexive**, **symétrique**, et **antisymétrique**.

---

### Exemple formel :

Soit l'ensemble $E = {1, 2, 3}$ et la relation $R$ définie par $xRy \iff x = y$.  
Les éléments de la relation sont :

$R={(1,1),(2,2),(3,3)}.R = \{(1,1), (2,2), (3,3)\}.R={(1,1),(2,2),(3,3)}$.

Cette relation est réflexive, symétrique et antisymétrique, comme expliqué ci-dessus.


