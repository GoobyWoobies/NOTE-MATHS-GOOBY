# 2. Domaine de définition

## Le principe

Le **domaine de définition** $D_f$ est l'ensemble des $x$ pour lesquels on peut calculer $f(x)$. Il faut donc repérer les calculs **interdits**.

## Les deux cas standards

### Les fractions

$$f(x) = \frac{g(x)}{h(x)} \quad\Rightarrow\quad h(x) \neq 0$$

On ne divise jamais par $0$.

> 💡 Bon à savoir : la fraction vaut $0$ seulement si son **numérateur** vaut $0$ (et que le dénominateur est non nul).

### Les racines paires

$$f(x) = \sqrt[n]{g(x)} \text{ avec } n \text{ pair} \quad\Rightarrow\quad g(x) \geq 0$$

On ne prend pas la racine carrée d'un nombre négatif (dans $\mathbb{R}$).

## ✏️ Exemples

| Fonction | Condition | Domaine |
| --- | --- | --- |
| $f(x) = \dfrac{1}{x-2}$ | $x - 2 \neq 0$ | $D_f = \mathbb{R}\setminus\{2\}$ |
| $f(x) = \sqrt{x-3}$ | $x - 3 \geq 0$ | $D_f = [3\,;\,+\infty[$ |
| $f(x) = \dfrac{\sqrt{x}}{x-1}$ | $x \geq 0$ **et** $x \neq 1$ | $D_f = [0\,;\,1[\ \cup\ ]1\,;\,+\infty[$ |

### Exemple avec un tableau des signes

Domaine de $f(x) = \sqrt{x^2-1}$.

Condition : $x^2 - 1 \geq 0$. D'après le [tableau des signes](../Algebre/08-tableau-des-signes.md), cette expression est positive ou nulle pour $x \leq -1$ ou $x \geq 1$.

$$D_f = ]-\infty\,;\,-1]\ \cup\ [1\,;\,+\infty[$$
