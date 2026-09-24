# 8. Le tableau des signes

## À quoi ça sert ?

À savoir **où** une expression est positive ($>0$), négative ($<0$) ou nulle. Il est indispensable pour :

- enlever une valeur absolue,
- résoudre une inéquation,
- trouver un domaine de définition (racines paires).

## La méthode

1. **Factoriser** l'expression (c'est le gros avantage : des facteurs simples ont des signes faciles).
2. **Trouver les zéros** de chaque facteur (là où il vaut $0$).
3. **Ranger** ces valeurs dans l'ordre croissant : elles découpent la droite en intervalles.
4. **Donner le signe** de chaque facteur sur chaque intervalle.
5. **Multiplier les signes** : $(+)\times(+) = +$, $(-)\times(-) = +$, $(+)\times(-) = -$.

## ✏️ Exemple : signe de $x^2 - 1$

**Étape 1 : factoriser** avec l'identité remarquable $a^2 - b^2 = (a+b)(a-b)$ :

$$x^2 - 1 = (x+1)(x-1)$$

**Étape 2 : zéros.** $(x+1)(x-1) = 0$ donne $x = -1$ ou $x = 1$.

**Étapes 3 à 5 : le tableau.**

| | $x < -1$ | $-1 < x < 1$ | $x > 1$ |
| --- | :---: | :---: | :---: |
| $x+1$ | $-$ | $+$ | $+$ |
| $x-1$ | $-$ | $-$ | $+$ |
| $(x+1)(x-1)$ | $+$ | $-$ | $+$ |

Aux valeurs $x = -1$ et $x = 1$, l'expression vaut $0$.

> 💡 **Vérification rapide** : on teste un nombre. Pour $x = 0$ : $0^2 - 1 = -1 < 0$ ✅ (cohérent avec la colonne du milieu).

## Conclusion

- $x^2 - 1 \geq 0$ sur $]-\infty\,;\,-1] \cup [1\,;\,+\infty[$
- $x^2 - 1 < 0$ sur $]-1\,;\,1[$

On en déduit la valeur absolue :

$$\lvert x^2-1\rvert = \begin{cases} x^2-1 & \text{si } x \leq -1 \text{ ou } x \geq 1 \\ -(x^2-1) & \text{si } -1 < x < 1 \end{cases}$$
