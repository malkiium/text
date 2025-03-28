#Limites #AlgèbreDeBase #MPSI #Informatique #LimiteSuite #LimiteFonction #PropriétésDesLimites #OpérationsLimites #TechniquesCalculLimites #FormesIndéterminées #LHopital #Gendarmes #Croissance #ExemplesMathématiques #Analyse #CalculLimites

## Définition de la Limite d'une Suite

Une suite Un  admet une limite  l  lorsque :
$$
\forall \varepsilon > 0, \exists N \in \mathbb{N}, \forall n \geq N, |u_n - l| < \varepsilon.$$
in other words:
For all epsilon greater than 0, there exists an N in the natural numbers, such that for all n greater than or equal to N, the absolute value of $$u_n - l$$ is less than epsilon.

Notation : $$ \lim\limits_{n \to +\infty} u_n = l $$.

## Définition de la Limite d'une Fonction

Une fonction  f admet une limite  l  en  a  si :       $\forall \varepsilon > 0, \exists \delta > 0, \forall x \in D_f, 0 < |x-a| < \delta \Rightarrow |f(x) - l| < \varepsilon.$
Notation :     $\lim\limits_{x \to a} f(x) = l$.
## Limites Usuelles

### Limites de Suites

- $\lim\limits_{n \to +\infty} \frac{1}{n} = 0$
- $\lim\limits_{n \to +\infty} r^n = 0$ si $|r| < 1$
- $\lim\limits_{n \to +\infty} n^p = +\infty$ pour tout $p > 0$
- $\lim\limits_{n \to +\infty} a^n = +\infty$ si $a > 1$

### Limites de Fonctions

- $\lim\limits_{x \to +\infty} \frac{1}{x} = 0$
- $\lim\limits_{x \to 0} \frac{1}{x} = +\infty$ (si $x > 0$) et $-\infty$ (si $x < 0$)
- $\lim\limits_{x \to +\infty} e^x = +\infty$ et $\lim\limits_{x \to -\infty} e^x = 0$

---

## Propriétés des Limites

### Opérations sur les Limites

Si $\lim\limits_{n \to +\infty} u_n = l$ et $\lim\limits_{n \to +\infty} v_n = m$, alors :

- $\lim\limits_{n \to +\infty} (u_n + v_n) = l + m$
- $\lim\limits_{n \to +\infty} (u_n \cdot v_n) = l \cdot m$
- $\lim\limits_{n \to +\infty} \frac{u_n}{v_n} = \frac{l}{m}$ si $m \neq 0$

### Formes Indéterminées

Certaines limites nécessitent des transformations (factorisation, conjugaison, développement limité, etc.) :

- $\frac{\infty}{\infty}$
- $\infty - \infty$
- $0 \times \infty$
- $0^0, \infty^0, 1^\infty$

---

## Techniques de Calcul de Limites

- **Factorisation** : Utilisation de la plus grande puissance pour simplifier.
- **Développement Limité** : Approximations pour exprimer un comportement asymptotique.
- **L'Hôpital** : Utilisation de  
    $lim⁡x→af(x)g(x)=lim⁡x→af′(x)g′(x)\lim\limits_{x \to a} \frac{f(x)}{g(x)} = \lim\limits_{x \to a} \frac{f'(x)}{g'(x)}x→alim​g(x)f(x)​=x→alim​g′(x)f′(x)$​  
    en cas de forme indéterminée $\frac{0}{0}$ ou $\frac{\infty}{\infty}$.
- **Encadrement (Théorème des Gendarmes)** :  
    Si $u_n \leq v_n \leq w_n$ et  
    $lim⁡n→+∞un=lim⁡n→+∞wn=l,\lim\limits_{n \to +\infty} u_n = \lim\limits_{n \to +\infty} w_n = l,n→+∞lim​un​=n→+∞lim​wn​=l,$
    alors  
    $lim⁡n→+∞vn=l.\lim\limits_{n \to +\infty} v_n = l.n→+∞lim​vn​=l.$

---

## Limites et Comparaison de Croissance

- $\ln x \ll x^a \ll a^x \ll x! \ll x^x$ pour $x \to +\infty$
- Comparaison entre exponentielle, polynôme, factorielle et puissance.

---

## Exemples et Exercices

1. Calculer  
    $lim⁡x→+∞x2+xx2−1.\lim\limits_{x \to +\infty} \frac{x^2 + x}{x^2 - 1}.x→+∞lim​x2−1x2+x​.$
2. Étudier la limite de  
    $un=(1+1n)n.u_n = \left( 1 + \frac{1}{n} \right)^n.un​=(1+n1​)n.$
3. Déterminer  
    $lim⁡x→0sin⁡xx.\lim\limits_{x \to 0} \frac{\sin x}{x}.x→0lim​xsinx​.$

## Conclusion

Les limites sont essentielles en analyse et en algèbre. Elles permettent de comprendre les comportements asymptotiques des suites et des fonctions, ce qui est fondamental pour la continuité, la dérivation et l'intégration.