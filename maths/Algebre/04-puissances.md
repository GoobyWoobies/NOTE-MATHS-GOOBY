# 4. Les puissances

## Rappel

$a^n$ signifie « $a$ multiplié $n$ fois par lui-même » : $2^3 = 2 \times 2 \times 2 = 8$.

## Règles générales

Soit $a$ et $b$ deux nombres **positifs**, et $r$ et $s$ des nombres rationnels. Alors :

| N° | Règle | Exemple |
| --- | --- | --- |
| 1 | $a^r \cdot a^s = a^{r+s}$ | $2^3 \cdot 2^2 = 2^5 = 32$ |
| 2 | $\dfrac{a^r}{a^s} = a^{r-s}$ | $\dfrac{3^5}{3^2} = 3^3 = 27$ |
| 3 | $(a^r)^s = a^{r\cdot s}$ | $(2^3)^2 = 2^6 = 64$ |
| 4 | $(a\,b)^r = a^r\,b^r$ | $(2\cdot 5)^2 = 4 \cdot 25 = 100$ |
| 5 | $\left(\dfrac{a}{b}\right)^r = \dfrac{a^r}{b^r}$ avec $b \neq 0$ | $\left(\dfrac{2}{3}\right)^2 = \dfrac{4}{9}$ |

> 💡 **Moyen mnémotechnique** : quand on **multiplie** des puissances de même base, on **additionne** les exposants. Quand on **divise**, on **soustrait**.

## Astuces

**Exposant négatif** : un exposant négatif « retourne » la puissance.

$$a^{-n} = \frac{1}{a^n}$$

✏️ $2^{-3} = \dfrac{1}{2^3} = \dfrac{1}{8}$

**Exposant nul** : $a^0 = 1$ pour tout $a \neq 0$.

> ⚠️ **Cas particulier** : $0^0$ **n'est pas défini**.

**Exposant fractionnaire** : il fait le lien avec les racines (voir le [chapitre suivant](05-racines.md)).

$$a^{\frac{p}{q}} = \sqrt[q]{a^{p}}$$

## ✏️ Exemple complet

Simplifier $\dfrac{(x^2)^3 \cdot x^{-4}}{x}$.

1. $(x^2)^3 = x^{6}$ (règle 3)
2. $x^6 \cdot x^{-4} = x^{2}$ (règle 1)
3. $\dfrac{x^2}{x} = x^{2-1} = x$ (règle 2)

Résultat : $x$.
