#relations-binaires #propriétés #relation-ordre #relation-équivalence #mathématiques #informatique
# Relations Binaires : L'essentiel

## Définition
Une **relation binaire** sur un ensemble $E$ est un **sous-ensemble** de $E \times E$, c'est-à-dire un ensemble de couples $(x, y)$.

---

## Propriétés des Relations Binaires

- **Réflexive** : $\forall x \in E, (x, x) \in R$
  - Chaque élément est en relation avec lui-même.
  
- **Symétrique** : $\forall x, y \in E, (x, y) \in R \Rightarrow (y, x) \in R$
  - Si $x$ est lié à $y$, alors $y$ est lié à $x$.

- **Antisymétrique** : $\forall x, y \in E, (x, y) \in R$ et $(y, x) \in R \Rightarrow x = y$
  - Si  x \neq y$, alors au plus un seul des couples $(x, y)$ ou $(y, x)$ est dans $R$.

- **Transitive** : $\forall x, y, z \in E, (x, y) \in R$ et $(y, z) \in R \Rightarrow (x, z) \in R$
  - Si $x$ est lié à $y$ et $y$ est lié à $z$, alors $x$ est lié à $z$.

---

## Types Importants de Relations

- **Relation d'équivalence** : Réflexive + Symétrique + Transitive  
  → Exemple : "avoir la même couleur de cheveux".  
  
- **Relation d'ordre** : Réflexive + Antisymétrique + Transitive  
  → Exemple : "être plus petit ou égal" $\leq$ .  
  
- **Relation strictement d'ordre** : Antisymétrique + Transitive  
  → Exemple : "être strictement inférieur" $<$.  
  
- **Relation de préordre** : Réflexive + Transitive  
  → Exemple : "être au moins aussi grand que".

---

## Ensembles Ordonnés

Un **ensemble ordonné** est un ensemble $E$ muni d'une relation d'ordre $R$.

- **Ordre total** : Tout couple $(x, y)$ d'éléments de $E$ est comparable, c'est-à-dire que $x R y$ ou $y R x$.  
  → Exemple : $\leq$ sur $\mathbb{R}$.

- **Ordre partiel** : Certains éléments de $E$ peuvent être incomparables.  
  → Exemple : $\subseteq$ sur l'ensemble des parties d'un ensemble.

Un **treillis** est un ensemble ordonné dans lequel chaque paire d'éléments admet un **supremum** (plus petit majorant) et un **infimum** (plus grand minorant).

### Ordre Produit et Ordre Lexicographique

- **Ordre produit** : Si $(E, \leq_E)$ et $(F, \leq_F)$ sont deux ensembles ordonnés, l'ordre produit sur $E \times F$ est défini par :  
  $$(x_1, y_1) \leq (x_2, y_2) \iff x_1 \leq_E x_2 \text{ et } y_1 \leq_F y_2.$$  
  → Exemple : Sur $ \mathbb{R}^2 $ avec l'ordre usuel sur $ \mathbb{R} $, l'ordre produit compare indépendamment chaque coordonnée.

- **Ordre lexicographique** : Défini sur $E \times F$ par :  
  $$(x_1, y_1) \leq (x_2, y_2) \iff x_1 < x_2 \text{ ou } (x_1 = x_2 \text{ et } y_1 \leq y_2).$$  
  → Exemple : L'ordre des mots dans un dictionnaire suit l'ordre lexicographique.

---

## Représentation d'une Relation

- **Matrice d'adjacence** : Tableau où une case $(i, j)$ est 1 si $(x_i, x_j)$ est dans $ R $, sinon 0.
- **Graphe orienté** : Sommets représentant les éléments de $ E $ et flèches pour les couples $(x, y)$.

- **Diagramme de Hasse** : Représentation simplifiée d'un ordre partiel. Il s'agit d'un graphe orienté acyclique où :
  - Les sommets représentent les éléments de $E$.
  - Une arête entre $x$ et $y$ signifie que $x \leq y$, sans passer par des intermédiaires.
  - Les arêtes sont généralement orientées vers le haut pour représenter la hiérarchie.
  
Exemple : Le diagramme de Hasse de $\{1,2,3,6\}$ avec la relation "divise" contient les arêtes $1 \to 2$, $1 \to 3$, et $2,3 \to 6$.

---

## Exemples Courants

- **Relation d'équivalence** : Congruence modulo $n$, appartenance à une même classe.
- **Relation d'ordre** : $\subseteq$ sur l'ensemble des parties d'un ensemble, $\leq$ sur $\mathbb{N}$.

---

**Résumé** : Une relation binaire est un sous-ensemble de $E \times E$. Selon ses propriétés, elle peut être une relation d'équivalence ou d'ordre, avec diverses applications en mathématiques et informatique.
