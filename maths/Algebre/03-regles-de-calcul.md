# 3. Règles de calcul

## Attention à la notation

On ne met **jamais deux opérateurs côte à côte**.

- ❌ $\times -1$
- ✅ $\times (-1)$

Les parenthèses évitent toute confusion entre l'opération (« fois ») et le signe (« moins »).

## La « Feinte du loup » (FDL)

C'est une technique pour **simplifier** une expression sans changer sa valeur. Le principe : on utilise deux « neutres » qui ne modifient rien.

| Neutre | Pourquoi ça ne change rien | Opération |
| --- | --- | --- |
| $0$ | $a + 0 = a$ | on **ajoute** $0$ (sous la forme $+1-1$, $+2-2$…) |
| $1$ | $a \times 1 = a$ et $\dfrac{a}{1} = a$ | on **multiplie** ou on **divise** par $1$ (sous la forme $\dfrac{c}{c}$) |

### Option 1 : ajouter $0$

**But** : faire apparaître au numérateur la même expression qu'au dénominateur.

✏️ **Exemple** : simplifier $\dfrac{x}{x-1}$.

1. On écrit $x = (x-1) + 1$ (on a ajouté $-1+1 = 0$).
2. Donc $\dfrac{x}{x-1} = \dfrac{(x-1)+1}{x-1}$.
3. On sépare la fraction : $\dfrac{x-1}{x-1} + \dfrac{1}{x-1}$.
4. On simplifie : $\dfrac{x-1}{x-1} = 1$.

$$\frac{x}{x-1} = 1 + \frac{1}{x-1}$$

✏️ **Autre exemple** : $\dfrac{x+3}{x+1} = \dfrac{(x+1)+2}{x+1} = 1 + \dfrac{2}{x+1}$.

### Option 2 : multiplier ou diviser par $1$

On choisit un « $1$ » déguisé, par exemple $\dfrac{3}{3}$, pour obtenir un **dénominateur commun**.

✏️ **Exemple** : $\dfrac{1}{2} + \dfrac{1}{3} = \dfrac{1}{2}\times\dfrac{3}{3} + \dfrac{1}{3}\times\dfrac{2}{2} = \dfrac{3}{6} + \dfrac{2}{6} = \dfrac{5}{6}$.

### Règle associée : séparer une fraction

Quand le **numérateur** est une somme et le dénominateur un seul terme :

$$\frac{a+b}{c} = \frac{a}{c} + \frac{b}{c}$$

> ⚠️ **Attention** : cela ne marche **pas** dans l'autre sens. $\dfrac{a}{b+c} \neq \dfrac{a}{b} + \dfrac{a}{c}$.

## Les identités remarquables

Trois formules à connaître par cœur : elles servent à **développer** (enlever les parenthèses) et à **factoriser** (les remettre).

$$(a+b)^2 = a^2 + 2ab + b^2$$

$$(a-b)^2 = a^2 - 2ab + b^2$$

$$(a+b)(a-b) = a^2 - b^2$$

> ⚠️ **Erreur classique** : $(a+b)^2 \neq a^2 + b^2$. Il ne faut pas oublier le terme du milieu $2ab$.

✏️ **Exemples**

- $(x+3)^2 = x^2 + 6x + 9$
- $(2x-1)^2 = 4x^2 - 4x + 1$
- $(x+1)(x-1) = x^2 - 1$ ← très utile pour le [tableau des signes](08-tableau-des-signes.md)

Dans l'autre sens (factoriser) : $x^2 - 9 = (x+3)(x-3)$.
