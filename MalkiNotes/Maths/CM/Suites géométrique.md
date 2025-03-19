# suite géométriques
---

## Limite des suites géométriques

### Définition d'une suite géométrique  
Une suite $u_n$ est dite **géométrique** s'il existe un réel $q$ tel que :  
$u_{n+1} = q \cdot u_n$

Le terme général d'une suite géométrique est donné par la formule :  
$u_n = u_1 \cdot q^{n-1}$

où :
- $u_1$ est le premier terme de la suite,
- $q$ est la raison de la suite.

### Limite d'une suite géométrique  
La limite de la suite $u_n$ dépend de la valeur de $q$ :

- Si $|q| < 1$, alors :
$\lim_{n \to \infty} u_n = 0$

- Si $|q| > 1$, alors :
$\lim_{n \to \infty} u_n = \infty$ si $u_1 > 0$

- Si  $q=1$, alors la suite est **constante** : $u_n = u_1$.

- Si $q = -1$, alors la suite **alterne** entre $u_1$ et $-u_1$ et **n'admet pas de limite**.

### Exemple avec \( q = 2 \)  
Si $u_n = 2^{n-1}$, alors :
$\lim_{n \to \infty} 2^{n-1} = \infty$

La suite croît **exponentiellement**.