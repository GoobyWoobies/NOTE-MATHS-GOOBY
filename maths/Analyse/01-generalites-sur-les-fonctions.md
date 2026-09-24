# 1. Généralités sur les fonctions

## Qu'est-ce qu'une fonction ?

Une **fonction** est une relation qui associe à chaque valeur $x$ d'un ensemble $A$ **une seule** valeur $y$ d'un ensemble $B$.

- $A$ = **ensemble de définition** (les $x$ autorisés)
- $B$ = **ensemble image** (les $y$ obtenus)

On pense souvent à une **machine** : on met $x$ à l'entrée, et il sort $y = f(x)$.

> 💡 **À retenir** : à un $x$ correspond **toujours un seul** $y$. En revanche, un même $y$ peut venir de plusieurs $x$ différents (par exemple $f(x)=x^2$ donne $4$ pour $x=2$ et pour $x=-2$).

## Image et préimage

Dans le graphique d'une fonction :

- $y$ s'appelle l'**image** de $x$,
- $x$ s'appelle la **préimage** de $y$ (on dit aussi *antécédent*).

✏️ Si $f(x) = x^2$ : l'image de $3$ est $9$, et les préimages de $9$ sont $3$ et $-3$.

## Quatre façons de décrire une fonction

| Manière | Exemple |
| --- | --- |
| **Verbalement** | « L'élongation d'un ressort est proportionnelle à la force qui lui est appliquée. » |
| **Tableau de mesures** (la « boîte noire ») | voir ci-dessous |
| **Graphiquement** | une courbe dans le plan $(x, y)$ |
| **Expression algébrique** | $f(x) = 2x + 1$ |

✏️ **Tableau de mesures** pour $f(x) = 2x+1$ :

| $x$ | $0$ | $1$ | $2$ | $3$ |
| --- | --- | --- | --- | --- |
| $f(x)$ | $1$ | $3$ | $5$ | $7$ |

## Domaine et ensemble image

Si rien n'est précisé, on prend pour $A$ et $B$ les ensembles **naturels** de définition et d'image. On les note :

- $D_f$ : le domaine de définition (les $x$ possibles),
- $\mathrm{Im}_f$ : l'ensemble image (les $y$ atteints).

✏️ **Exemple** : $f(x) = \dfrac{1}{x}$

- Il y a **une valeur interdite** : $x \neq 0$ (on ne divise pas par zéro). Toutes les autres marchent, donc $D_f = \mathbb{R}^*$.
- On peut atteindre n'importe quel $y$ sauf $0$ (car $\frac{1}{x}$ ne vaut jamais $0$). Donc $\mathrm{Im}_f = \mathbb{R}^*$.

➡️ Suite : [comment trouver le domaine de définition](02-domaine-de-definition.md).
