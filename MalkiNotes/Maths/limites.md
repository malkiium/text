# Limites en Algèbre de Base (MPSI - Informatique)

## Définition de la Limite d'une Suite

Une suite \( (u_n) \) admet une limite \( l \) lorsque :
\[
\forall \varepsilon > 0, \exists N \in \mathbb{N}, \forall n \geq N, |u_n - l| < \varepsilon.
\]
Notation : \( \lim\limits_{n \to +\infty} u_n = l \).

## Définition de la Limite d'une Fonction

Une fonction \( f \) admet une limite \( l \) en \( a \) si :
\[
\forall \varepsilon > 0, \exists \delta > 0, \forall x \in D_f, 0 < |x-a| < \delta \Rightarrow |f(x) - l| < \varepsilon.
\]
Notation : \( \lim\limits_{x \to a} f(x) = l \).

## Limites Usuelles

### Limites de Suites

- \( \lim\limits_{n \to +\infty} \frac{1}{n} = 0 \)
- \( \lim\limits_{n \to +\infty} r^n = 0 \) si \( |r| < 1 \)
- \( \lim\limits_{n \to +\infty} n^p = +\infty \) pour tout \( p > 0 \)
- \( \lim\limits_{n \to +\infty} a^n = +\infty \) si \( a > 1 \)

### Limites de Fonctions

- \( \lim\limits_{x \to +\infty} \frac{1}{x} = 0 \)
- \( \lim\limits_{x \to 0} \frac{1}{x} = +\infty \) (si \( x > 0 \)) et \( -\infty \) (si \( x < 0 \))
- \( \lim\limits_{x \to +\infty} e^x = +\infty \) et \( \lim\limits_{x \to -\infty} e^x = 0 \)

## Propriétés des Limites

### Opérations sur les Limites

Si \( \lim\limits_{n \to +\infty} u_n = l \) et \( \lim\limits_{n \to +\infty} v_n = m \), alors :

- \( \lim\limits_{n \to +\infty} (u_n + v_n) = l + m \)
- \( \lim\limits_{n \to +\infty} (u_n \cdot v_n) = l \cdot m \)
- \( \lim\limits_{n \to +\infty} \frac{u_n}{v_n} = \frac{l}{m} \) si \( m \neq 0 \)

### Formes Indéterminées

Certaines limites nécessitent des transformations (factorisation, conjugaison, développement limité, etc.) :

- \( \frac{\infty}{\infty} \)
- \( \infty - \infty \)
- \( 0 \times \infty \)
- \( 0^0, \infty^0, 1^\infty \)

## Techniques de Calcul de Limites

- **Factorisation** : Utilisation de la plus grande puissance pour simplifier.
- **Développement Limité** : Approximations pour exprimer un comportement asymptotique.
- **L'Hôpital** : Utilisation de \( \lim\limits_{x \to a} \frac{f(x)}{g(x)} = \lim\limits_{x \to a} \frac{f'(x)}{g'(x)} \) en cas de forme indéterminée \( \frac{0}{0} \) ou \( \frac{\infty}{\infty} \).
- **Encadrement (Théorème des Gendarmes)** : Si \( u_n \leq v_n \leq w_n \) et \( \lim\limits_{n \to +\infty} u_n = \lim\limits_{n \to +\infty} w_n = l \), alors \( \lim\limits_{n \to +\infty} v_n = l \).

## Limites et Comparaison de Croissance

- \( \ln x \ll x^a \ll a^x \ll x! \ll x^x \) pour \( x \to +\infty \)
- Comparaison entre exponentielle, polynôme, factorielle et puissance

## Exemples et Exercices

1. Calculer \( \lim\limits_{x \to +\infty} \frac{x^2 + x}{x^2 - 1} \).
2. Étudier la limite de \( u_n = \left( 1 + \frac{1}{n} \right)^n \).
3. Déterminer \( \lim\limits_{x \to 0} \frac{\sin x}{x} \).

## Conclusion

Les limites sont essentielles en analyse et en algèbre. Elles permettent de comprendre les comportements asymptotiques des suites et des fonctions, ce qui est fondamental pour la continuité, la dérivation et l'intégration.
