# 6. La valeur absolue

## L'idée

La **valeur absolue** d'un nombre $a$, notée $\lvert a\rvert$, est sa **distance à $0$** sur la droite réelle. Une distance est toujours positive ou nulle :

$$\lvert a\rvert \geq 0 \quad \text{pour tout nombre } a$$

## Définition

$$\lvert a\rvert = \begin{cases} a & \text{si } a \geq 0 \\ -a & \text{si } a < 0 \end{cases}$$

✏️ **Exemple** : $\lvert -3\rvert = 3$, car $-3 < 0$ donc $\lvert -3\rvert = -(-3) = +3$.

> 💡 **À retenir** : la valeur absolue « enlève le signe moins ». Elle ne rend pas $-a$ mais bien un nombre positif : si $a$ est négatif, $-a$ est positif.

## Lien avec la racine carrée

$$\sqrt{x^2} = \lvert x\rvert$$

✏️ **Exemple** : $\sqrt{(-3)^2} = \sqrt{9} = 3 = \lvert -3\rvert$.

> ⚠️ **Attention aux parenthèses**
> - $(-3)^2 = 9$ (le carré s'applique à $-3$)
> - $-3^2 = -9$ (le carré s'applique seulement à $3$)

### Racines $n$-ièmes

- $\sqrt[n]{A^n} = A$ si $n$ est **impair**
- $\sqrt[n]{A^n} = \lvert A\rvert$ si $n$ est **pair**

## Propriétés

Pour deux réels $a$ et $b$ quelconques et un entier $n$ :

1. $\lvert a\,b\rvert = \lvert a\rvert \cdot \lvert b\rvert$
2. $\left\lvert \dfrac{a}{b} \right\rvert = \dfrac{\lvert a\rvert}{\lvert b\rvert}$ avec $b \neq 0$
3. $\lvert a^n\rvert = \lvert a\rvert^n$

> ⚠️ En général $\lvert a+b\rvert \neq \lvert a\rvert + \lvert b\rvert$. Exemple : $\lvert 2 + (-5)\rvert = 3$ mais $\lvert 2\rvert + \lvert -5\rvert = 7$.

## Résoudre avec une valeur absolue

Pour $a > 0$ :

| Si on a… | … alors |
| --- | --- |
| $\lvert x\rvert = a$ | $x = a$ **ou** $x = -a$, soit $x = \pm a$ |
| $\lvert x\rvert < a$ | $-a < x < a$ |
| $\lvert x\rvert > a$ | $x > a$ **ou** $x < -a$ |

### ✏️ Exemple 1 : $x^2 = 9$

On prend la racine carrée des deux côtés : $\sqrt{x^2} = \sqrt{9}$, donc $\lvert x\rvert = 3$.

- Si $x \geq 0$ : $\lvert x\rvert = x$, donc $x = 3$.
- Si $x < 0$ : $\lvert x\rvert = -x$, donc $-x = 3$, soit $x = -3$.

**Solutions** : $x = \pm 3$.

> ⚠️ Ne jamais écrire seulement $x = 3$ : on **perd** la solution négative.

### ✏️ Exemple 2 : $\lvert x-1\rvert < 3$

$-3 < x-1 < 3$, on ajoute $1$ partout : $-2 < x < 4$. Solution : $x \in ]-2\,;\,4[$.

### ✏️ Exemple 3 : $\sqrt{(x^2-1)^2}$

On applique $\sqrt{A^2} = \lvert A\rvert$ avec $A = x^2 - 1$ :

$$\sqrt{(x^2-1)^2} = \lvert x^2-1\rvert = \begin{cases} x^2-1 & \text{si } x^2-1 \geq 0 \\ -(x^2-1) & \text{si } x^2-1 < 0 \end{cases}$$

Pour savoir quand $x^2-1$ est positif ou négatif, on utilise un **tableau des signes** → [chapitre 8](08-tableau-des-signes.md).
