# 1. Les ensembles de nombres

## L'idée

Les nombres sont rangés dans des « boîtes » de plus en plus grandes. Chaque boîte contient la précédente.

| Ensemble | Symbole | Ce qu'il contient | Exemples |
| --- | --- | --- | --- |
| Naturels | $\mathbb{N}$ | les nombres pour compter | $0,\ 1,\ 2,\ 3,\dots$ |
| Entiers | $\mathbb{Z}$ | les naturels et leurs opposés (négatifs) | $\dots,-2,\ -1,\ 0,\ 1,\ 2,\dots$ |
| Rationnels | $\mathbb{Q}$ | les fractions | $\dfrac{1}{2},\ -\dfrac{7}{3},\ 0{,}75$ |
| Réels | $\mathbb{R}$ | tous les nombres de la droite numérique | $\sqrt{2},\ \pi,\ -4,\ \dfrac{1}{3}$ |

## Les boîtes s'emboîtent

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$$

Cela se lit : « les naturels sont inclus dans les entiers, qui sont inclus dans les rationnels, qui sont inclus dans les réels ».

> 💡 **À retenir** : un nombre comme $\sqrt{2}$ ou $\pi$ est **réel** mais **pas rationnel** : on ne peut pas l'écrire comme une fraction.
>
> (Au-dessus de $\mathbb{R}$, il existe encore les nombres complexes $\mathbb{C}$, qui ne sont pas au programme ici.)

## La droite numérique

Tous les nombres réels se placent sur une droite : chaque point de la droite correspond à **un** réel, et chaque réel à **un** point.

Avec la notion d'intervalle (voir le [chapitre suivant](02-symboles-et-intervalles.md)), l'ensemble des réels s'écrit :

$$\mathbb{R} = \left]-\infty ;\ +\infty\right[$$

## Notations pratiques

| Notation | Signification | Exemple |
| --- | --- | --- |
| $\mathbb{R}^*$ | les réels **sans le zéro** : $\mathbb{R}\setminus\{0\}$ | $-5 \in \mathbb{R}^*$, mais $0 \notin \mathbb{R}^*$ |
| $\mathbb{R}_+$ | les réels **positifs** (zéro compris) | $0 \in \mathbb{R}_+$, $3 \in \mathbb{R}_+$ |

Le symbole $\setminus$ se lit « privé de » : $\mathbb{R}\setminus\{0\}$ = « les réels privés de zéro ».
