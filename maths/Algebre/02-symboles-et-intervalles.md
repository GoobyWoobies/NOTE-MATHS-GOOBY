# 2. Symboles et intervalles

## Le vocabulaire des symboles

| Symbole | Se lit | Exemple |
| --- | --- | --- |
| $\forall$ | pour tout | $\forall x \in \mathbb{R},\ x^2 \geq 0$ |
| $\exists$ | il existe | $\exists x \in \mathbb{R},\ x + 3 = 5$ |
| $\nexists$ | il n'existe pas | $\nexists x \in \mathbb{R},\ x^2 = -1$ |
| $\in$ | appartient à (« est un élément de ») | $3 \in \mathbb{N}$ |
| $\cup$ | réunion (« ou ») | $A \cup B$ : dans $A$ **ou** dans $B$ |
| $\cap$ | intersection (« et ») | $A \cap B$ : dans $A$ **et** dans $B$ |

> ⚠️ **Attention à ne pas confondre**
> - $\in$ relie un **élément** à un **ensemble** : $3 \in \mathbb{N}$.
> - $\subset$ relie un **ensemble** à un **ensemble** : $\mathbb{N} \subset \mathbb{Z}$.

## Les intervalles

Un **intervalle** décrit « tous les nombres compris entre deux bornes ».

| Notation | Inégalité | Signification |
| --- | --- | --- |
| $]a\,;\,b[$ | $a < x < b$ | **ouvert** : $a$ et $b$ **non compris** |
| $[a\,;\,b]$ | $a \leq x \leq b$ | **fermé** : $a$ et $b$ compris |
| $[a\,;\,b[$ | $a \leq x < b$ | fermé en $a$, ouvert en $b$ |
| $]a\,;\,+\infty[$ | $x > a$ | tout ce qui est plus grand que $a$ |
| $]-\infty\,;\,b]$ | $x \leq b$ | tout ce qui est plus petit ou égal à $b$ |

> 💡 **Règle d'or** : devant l'infini ($+\infty$ ou $-\infty$), le crochet est **toujours ouvert**, car l'infini n'est pas un nombre qu'on peut « atteindre ».

Si on a uniquement $-\infty$ et $+\infty$, on écrit simplement $\mathbb{R}$.

## ✏️ Exemples

- $x \in ]2\,;\,5[$ signifie $2 < x < 5$. Ici $3$ convient, mais $2$ et $5$ non.
- $x \in [-1\,;\,4]$ signifie $-1 \leq x \leq 4$. Ici $-1$ et $4$ conviennent.
- « $x \neq 0$ » s'écrit $x \in \mathbb{R}^* = ]-\infty\,;\,0[ \ \cup\ ]0\,;\,+\infty[$ : on utilise $\cup$ car $x$ est soit négatif, **ou** soit positif.
