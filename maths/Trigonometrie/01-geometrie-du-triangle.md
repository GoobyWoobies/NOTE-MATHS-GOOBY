# 1. Rappels de géométrie du triangle

## Objectifs

À la fin de ce chapitre, tu sais :

- nommer les sommets, côtés et angles d'un triangle avec les **conventions de notation** ;
- reconnaître les **triangles particuliers** (rectangle, isocèle, équilatéral) et repérer `hyp`, `opp`, `adj` ;
- utiliser les **relations fondamentales** : somme des angles et Pythagore ;
- reconnaître des **triangles semblables** et calculer une longueur avec le rapport de Thalès ;
- justifier que deux triangles sont **isométriques** (CCC, ACA, CAC).

> Source : module_1_trigonometrie.pdf, p. 1 (table des matières, partie 1)

## Prérequis

- Aucun chapitre précédent. Calcul avec fractions et racines carrées.

---

## Définitions

### 1.1 Triangle et conventions de notation

- Triangle $$\triangle ABC$$ → 3 **sommets** $$A$$, $$B$$, $$C$$
- **Segment** $$[AB]$$ → portion de droite entre $$A$$ et $$B$$
- **Longueur** $$\lvert AB \rvert$$ → distance entre $$A$$ et $$B$$ (un nombre)
- **Côtés** → lettre **minuscule du sommet opposé** :
  - $$a = \lvert BC \rvert$$ (en face de $$A$$)
  - $$b = \lvert AC \rvert$$ (en face de $$B$$)
  - $$c = \lvert AB \rvert$$ (en face de $$C$$)
- **Angles** → lettres grecques, même ordre :
  - $$\hat{A} = \alpha$$ ; $$\hat{B} = \beta$$ ; $$\hat{C} = \gamma$$

↳ l'angle $$\alpha$$ et le côté $$a$$ se font **face**, et c'est pareil pour $$\beta$$ et $$b$$, $$\gamma$$ et $$c$$.

**Notations que tu verras dans les tests** (même sens, autre écriture) :

- longueur : $$\overline{AD}$$ (TE de M. Hebeisen) ou $$\lvert AB \rvert$$ (tests de M. Janka)
- angle : $$\angle ADB$$ ou $$\widehat{BCD}$$ → l'angle **au sommet du milieu** (ici $$D$$, resp. $$C$$)

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01-geometrie-du-triangle.md ; notations des tests : Algebre_merged.pdf, p. 232 et p. 250

### 1.2 Triangles particuliers

| Triangle | Caractéristique |
| --- | --- |
| **Rectangle** | un angle de $$90^\circ$$ |
| **Isocèle** | deux côtés égaux (↳ les deux angles à la base sont égaux) |
| **Équilatéral** | trois côtés égaux et trois angles de $$60^\circ$$ |

**Triangle rectangle : les noms des côtés** (vus depuis un angle aigu $$\alpha$$) :

- `hyp` = **hypoténuse** → côté **en face de l'angle droit**, toujours le plus long
- `opp` = côté **opposé** à $$\alpha$$ → en face de $$\alpha$$
- `adj` = côté **adjacent** à $$\alpha$$ → touche $$\alpha$$, mais ce n'est pas `hyp`

⚠ `opp` et `adj` **dépendent de l'angle choisi** : si on regarde l'autre angle aigu, ils s'échangent. `hyp` ne change jamais.

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01-geometrie-du-triangle.md ; recap-trigo-manuscrit.pdf, p. 1 (hyp / opp / adj). La remarque sur les angles à la base du triangle isocèle est rédigée hors cours (style des notes).

### 1.3 Relations fondamentales

**Somme des angles**, valable dans **tout** triangle :

$$
\alpha + \beta + \gamma = 180^\circ
$$

**Théorème de Pythagore**, valable **uniquement** dans un triangle **rectangle**. Avec l'angle droit en $$C$$ (donc $$c$$ = `hyp`) :

$$
a^2 + b^2 = c^2
$$

↳ en mots : $$\text{hyp}^2 = \text{côté}_1^2 + \text{côté}_2^2$$

⚠ Dans les TE, les angles sont souvent en **radians** : la somme des angles s'écrit alors $$\alpha + \beta + \gamma = \pi$$ et l'angle droit vaut $$\frac{\pi}{2}$$ (conversion : [chapitre 2](02-angles.md)).

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01-geometrie-du-triangle.md ; usage des radians : Algebre_merged.pdf, p. 223, 232, 241

**Deux outils utilisés dans les tests** :

- **Angles sur une droite** → deux angles côte à côte sur une même droite font $$180^\circ$$ (supplémentaires)
  - Ex : si $$z = 90^\circ - \alpha$$, l'angle voisin sur la même droite vaut $$u = 180^\circ - z = 90^\circ + \alpha$$
- **Triangle dans un demi-cercle** → si $$[AC]$$ est un diamètre et $$D$$ est sur le demi-cercle, alors l'angle en $$D$$ est **droit**
  - ↳ « l'arc $$\widehat{ADC}$$ est un demi-cercle » = indice caché : $$\triangle ACD$$ est **rectangle en $$D$$** → Pythagore possible

{% hint style="info" %}
**Complément (hors cours).** Ces deux propriétés ne figurent pas dans tes notes, mais les corrections des tests les utilisent : le calcul de $$\widehat{BCD}$$ à partir des angles voisins (p. 250), et $$\overline{AC} = \sqrt{\overline{AD}^2 + \overline{DC}^2}$$ dès que l'énoncé parle de demi-cercle (p. 223, 232, 241).
{% endhint %}

> Source : Algebre_merged.pdf, p. 250 (Janka, Test 1 Pb 2, 2023/24) ; p. 223, 232, 241 (TE F-1 2022, 2023, 2025, Ex. 1)

### 1.4 Triangles semblables

- Deux triangles sont **semblables** s'ils ont **la même forme** mais pas forcément la même taille
  - ↳ mêmes angles
  - ↳ côtés **proportionnels** : tous multipliés par le même rapport $$k$$

**Théorème de Thalès** : dans $$\triangle ABC$$, avec $$D \in (AB)$$, $$E \in (AC)$$ et $$(DE) \parallel (BC)$$ :

$$
k = \frac{\lvert AD \rvert}{\lvert AB \rvert} = \frac{\lvert AE \rvert}{\lvert AC \rvert} = \frac{\lvert DE \rvert}{\lvert BC \rvert}
$$

↳ le petit triangle $$ADE$$ est une **réduction** du grand $$ABC$$.

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 03-thales.md

### 1.5 Triangles égaux ou isométriques

- **Isométriques** (= égaux, superposables) → même forme **et** même taille
  - ↳ on peut poser l'un exactement sur l'autre
  - notation : $$\triangle ABC \cong \triangle A'B'C'$$
- Ça veut dire **6 égalités** : 3 angles et 3 côtés
- **3 informations suffisent**, selon un des critères :

| Critère | Ce qu'il faut | Exemple |
| --- | --- | --- |
| **CCC** | les 3 côtés égaux | $$\lvert AB \rvert = \lvert A'B' \rvert$$, $$\lvert AC \rvert = \lvert A'C' \rvert$$, $$\lvert BC \rvert = \lvert B'C' \rvert$$ |
| **ACA** | 1 côté et les **2 angles qui le touchent** | $$\lvert BC \rvert = \lvert B'C' \rvert$$, $$\hat{B} = \hat{B}'$$, $$\hat{C} = \hat{C}'$$ |
| **CAC** | 2 côtés et l'**angle entre eux** | $$\lvert AB \rvert = \lvert A'B' \rvert$$, $$\lvert BC \rvert = \lvert B'C' \rvert$$, $$\hat{B} = \hat{B}'$$ |

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 02-triangles-isometriques.md

---

## Intuition

- **Somme = 180°** → les 3 angles « se partagent » un demi-tour. Donc si je connais 2 angles, j'ai automatiquement le 3ᵉ.
- **Pythagore** → dans un triangle rectangle, 2 côtés suffisent pour avoir le 3ᵉ.
  - ↳ c'est exactement ce qui fait marcher le cercle trigo plus tard : `hyp` = 1, donc $$x^2 + y^2 = 1$$
- **Semblables** → une photo agrandie ou réduite : les angles ne bougent pas, les longueurs sont multipliées par $$k$$.
  - ↳ c'est pour ça que $$\sin$$, $$\cos$$, $$\tan$$ (des **rapports**) ne dépendent que de l'angle, pas de la taille du triangle
- **Isométriques** → une photocopie à l'identique. 3 bonnes infos « bloquent » le triangle : on ne peut plus en dessiner un autre.

{% hint style="info" %}
**Complément (hors cours).** Le lien « triangles semblables ↳ sin, cos, tan ne dépendent que de l'angle » explique pourquoi tes notes disent que le rapport est « un nombre pur ».
{% endhint %}

> Source : rédigé hors cours (style des notes) ; recap-trigo-manuscrit.pdf, p. 1–2

## Propriétés / théorèmes

| Propriété | Énoncé | Condition |
| --- | --- | --- |
| Somme des angles | $$\alpha + \beta + \gamma = 180^\circ$$ | tout triangle |
| Pythagore | $$a^2 + b^2 = c^2$$ | triangle **rectangle** en $$C$$ |
| Thalès | $$\frac{\lvert AD \rvert}{\lvert AB \rvert} = \frac{\lvert AE \rvert}{\lvert AC \rvert} = \frac{\lvert DE \rvert}{\lvert BC \rvert}$$ | $$(DE) \parallel (BC)$$ |
| Isométrie | CCC, ACA ou CAC ⟹ $$\triangle ABC \cong \triangle A'B'C'$$ | un seul critère suffit |

**Réciproque de Pythagore** : si $$a^2 + b^2 = c^2$$, alors le triangle est rectangle (angle droit en face de $$c$$).
↳ on s'en sert pour **vérifier** si un triangle est rectangle.

{% hint style="info" %}
**Complément (hors cours).** La réciproque de Pythagore n'apparaît pas dans tes sources actuelles. Elle est ajoutée parce qu'elle sert à vérifier si un triangle est rectangle.
{% endhint %}

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01-geometrie-du-triangle.md, 02-triangles-isometriques.md, 03-thales.md ; réciproque : rédigé hors cours

## Marche à suivre

**A. Trouver un angle manquant**

1. Vérifier qu'on connaît **2 angles** du triangle
2. Poser $$\alpha + \beta + \gamma = 180^\circ$$
3. Isoler l'angle inconnu

**B. Trouver un côté avec Pythagore**

1. Vérifier que le triangle est **rectangle**
2. Repérer `hyp` (en face de l'angle droit)
3. Écrire $$\text{hyp}^2 = \text{côté}_1^2 + \text{côté}_2^2$$
4. Isoler l'inconnue, puis prendre la **racine positive** (une longueur est > 0)

**C. Trouver une longueur avec Thalès**

1. Vérifier le **parallélisme** (sinon Thalès ne s'applique pas)
2. Repérer petit triangle / grand triangle
3. Calculer $$k$$ avec deux côtés **connus** qui se correspondent
4. Écrire les rapports **dans le même ordre** (petit / grand) et isoler l'inconnue

**D. Montrer que deux triangles sont isométriques**

1. Lister les égalités connues (côtés, angles)
2. Chercher le critère qui colle : CCC, ACA (angles **aux extrémités** du côté) ou CAC (angle **entre** les côtés)
3. Conclure : $$\triangle ABC \cong \triangle A'B'C'$$ par le critère …

> Source : rédigé hors cours (style des notes), à partir des énoncés des anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01 à 03

## Exemples résolus

**Ex 1 : angle manquant.** $$\alpha = 50^\circ$$, $$\beta = 60^\circ$$, $$\gamma = ?$$

- On a 2 angles → on utilise la somme des angles (marche à suivre A)
- $$\gamma = 180^\circ - 50^\circ - 60^\circ = 70^\circ$$

**Ex 2 : Pythagore.** Triangle rectangle en $$C$$, $$a = 3$$, $$b = 4$$, $$c = ?$$

- Rectangle en $$C$$ → $$c$$ = `hyp` (en face de l'angle droit)
- $$c^2 = 3^2 + 4^2 = 9 + 16 = 25$$
- $$c = \sqrt{25} = 5$$ → on garde la racine **positive**, car c'est une longueur

**Ex 3 : l'échelle (comme dans les notes, mais avec Pythagore).** Une échelle doit atteindre une fenêtre à $$4\,\text{m}$$. Son pied est à $$1{,}5\,\text{m}$$ du mur. Quelle longueur d'échelle ?

- Mur ⊥ sol → triangle **rectangle**
- L'échelle est en face de l'angle droit → c'est `hyp`
- $$\text{hyp}^2 = 4^2 + 1{,}5^2 = 16 + 2{,}25 = 18{,}25$$
- $$\text{hyp} = \sqrt{18{,}25} \approx 4{,}27\,\text{m}$$
- ↳ ici on a **2 côtés** → Pythagore. Dans les notes, on avait **1 côté + 1 angle** (70°) → là il faut $$\sin$$ ou $$\csc$$ (chapitre 3)

**Ex 4 : Thalès.** $$(DE) \parallel (BC)$$, $$\lvert AD \rvert = 3$$, $$\lvert AB \rvert = 6$$, $$\lvert AE \rvert = 5$$, $$\lvert DE \rvert = 4$$. Trouver $$\lvert AC \rvert$$ et $$\lvert BC \rvert$$.

- Parallèles → Thalès OK
- $$k = \frac{\lvert AD \rvert}{\lvert AB \rvert} = \frac{3}{6} = \frac{1}{2}$$ → le petit triangle est 2× plus petit
- $$\frac{5}{\lvert AC \rvert} = \frac{1}{2}$$ ↳ $$\lvert AC \rvert = 10$$
- $$\frac{4}{\lvert BC \rvert} = \frac{1}{2}$$ ↳ $$\lvert BC \rvert = 8$$

**Ex 5 : TE F-1 (novembre 2023), « Triangle & Co. », partie i).** L'arc $$\widehat{ADC}$$ est un demi-cercle, avec $$\overline{AD} = 25$$ et $$\overline{DC} = \sqrt{131{,}25}$$. On trace la hauteur $$h$$ depuis $$D$$ sur $$[AC]$$, avec pied $$H$$. Calculer $$h$$ (2 chiffres après la virgule, calculs explicites).

- « Demi-cercle » → $$\triangle ACD$$ rectangle en $$D$$ → `hyp` $$= \overline{AC}$$
- Pythagore : $$\overline{AC} = \sqrt{\overline{AD}^2 + \overline{DC}^2} = \sqrt{625 + 131{,}25} = \sqrt{756{,}25} = 27{,}5$$
- $$\triangle ACD$$ et $$\triangle DHC$$ sont **semblables** :
  - ↳ tous deux rectangles (en $$D$$ et en $$H$$)
  - ↳ même angle en $$C$$
  - ↳ donc même 3ᵉ angle (somme = 180°)
- Côté en face de l'angle en $$C$$ divisé par `hyp`, dans chaque triangle : $$\frac{h}{\overline{DC}} = \frac{\overline{AD}}{\overline{AC}}$$
- $$h = \frac{25 \cdot \sqrt{131{,}25}}{27{,}5} \approx 10{,}41$$
- ↳ c'est le calcul de la correction : $$\frac{h}{25} = \frac{\sqrt{131{,}25}}{27{,}5}$$. La suite de l'exercice (les angles) utilise arcsin et la loi des sinus → chapitres 3 à 5.

> Source : Ex 1–2 : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01-geometrie-du-triangle.md ; Ex 3 : rédigé hors cours, inspiré de recap-trigo-manuscrit.pdf, p. 1 ; Ex 4 : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 03-thales.md ; Ex 5 : Algebre_merged.pdf, p. 232

## Pièges fréquents

- ⚠ **Pythagore seulement si rectangle.** Sinon → loi du cosinus (chapitre 4)
- ⚠ **`hyp` = en face de l'angle droit**, pas « le côté en bas » ni « le côté oblique au hasard »
- ⚠ `opp` / `adj` **changent** si on change d'angle
- ⚠ **3 angles égaux ≠ isométriques** → seulement **semblables** (la taille peut changer)
- ⚠ **ACA** : les 2 angles doivent toucher **le côté donné**
- ⚠ **CAC** : l'angle doit être **entre** les 2 côtés (sinon ça ne marche pas)
- ⚠ **Thalès** : rapports **dans le même ordre** (petit / grand partout), et parallélisme obligatoire
- ⚠ Racine carrée → garder **seulement le résultat positif** pour une longueur

**Pièges vus dans les tests :**

- ⚠ **Ne pas rater le triangle rectangle caché** (demi-cercle, hauteur, mur ⊥ sol). Correction du TE 2025 : « beaucoup plus simple avec triangle rectangle ! » → l'élève avait pris la loi du cosinus alors que $$\cos$$ dans le triangle rectangle suffisait
- ⚠ **Degrés ou radians** : les TE donnent $$\frac{\pi}{6}$$ et attendent des angles en rad. Ne mélange pas $$180^\circ$$ et $$\pi$$ dans le même calcul
- ⚠ « Précision de **deux chiffres après la virgule** » → arrondir **seulement à la fin**, garder $$\sqrt{131{,}25}$$ exact pendant le calcul
- ⚠ « Calculs explicites » → **une solution non développée est considérée comme fausse** (consigne de la page de garde des TE)

**Synthèse :**

- 2 angles connus → **somme = 180°** (ou $$\pi$$)
- triangle rectangle + 2 côtés → **Pythagore**
- droites parallèles → **Thalès** (rapport $$k$$)
- demi-cercle → **angle droit** → Pythagore
- 2 triangles avec 2 angles égaux → **semblables** → rapports égaux
- prouver « mêmes triangles » → **CCC / ACA / CAC**

> Source : anciennes notes Analyse 1 (supprimées, historique git 898580e) : 01 à 03 ; renvoi au chapitre 4 : module_1_trigonometrie.pdf, p. 1 (4.4) ; pièges des tests : Algebre_merged.pdf, p. 222 (consignes), 223, 232, 241

## Exercices

{% hint style="warning" %}
Aucune série d'exercices n'est encore dans `sources/exercices/`. Les exercices 1 à 5 sont **rédigés hors cours** (style des notes). Les exercices 6 à 9 viennent des **anciens tests** (`Algebre_merged.pdf`).
{% endhint %}

**Exercice 1.** Dans $$\triangle ABC$$ : $$\alpha = 35^\circ$$, $$\beta = 90^\circ$$. Calculer $$\gamma$$ et dire quel côté est `hyp`.

<details>
<summary>Indice</summary>

Somme des angles. Pour `hyp` : quel angle vaut 90° ? Quel côté est en face ?

</details>

<details>
<summary>Solution</summary>

- $$\gamma = 180^\circ - 35^\circ - 90^\circ = 55^\circ$$
- Angle droit en $$B$$ → `hyp` = côté en face de $$B$$ = $$b = \lvert AC \rvert$$

</details>

**Exercice 2.** Triangle rectangle : `hyp` $$= 13$$, un côté $$= 5$$. Trouver le 3ᵉ côté.

<details>
<summary>Indice</summary>

Cette fois l'inconnue n'est **pas** `hyp` : isole un côté dans $$\text{hyp}^2 = \text{côté}_1^2 + \text{côté}_2^2$$.

</details>

<details>
<summary>Solution</summary>

- $$13^2 = 5^2 + x^2$$ ↳ $$x^2 = 169 - 25 = 144$$
- $$x = \sqrt{144} = 12$$ (racine positive, c'est une longueur)

</details>

**Exercice 3.** Un triangle a des côtés $$6$$, $$8$$ et $$11$$. Est-il rectangle ?

<details>
<summary>Indice</summary>

Si oui, `hyp` serait le plus grand côté. Teste la réciproque de Pythagore.

</details>

<details>
<summary>Solution</summary>

- Plus grand côté = $$11$$ → on teste $$6^2 + 8^2 \overset{?}{=} 11^2$$
- $$36 + 64 = 100$$ et $$11^2 = 121$$
- $$100 \neq 121$$ → **pas rectangle**

</details>

**Exercice 4.** $$(DE) \parallel (BC)$$, $$\lvert AD \rvert = 2$$, $$\lvert AB \rvert = 5$$, $$\lvert DE \rvert = 3$$. Calculer $$\lvert BC \rvert$$.

<details>
<summary>Indice</summary>

Calcule d'abord $$k = \frac{\lvert AD \rvert}{\lvert AB \rvert}$$, puis utilise $$\frac{\lvert DE \rvert}{\lvert BC \rvert} = k$$.

</details>

<details>
<summary>Solution</summary>

- $$k = \frac{2}{5}$$
- $$\frac{3}{\lvert BC \rvert} = \frac{2}{5}$$ ↳ $$\lvert BC \rvert = \frac{3 \cdot 5}{2} = 7{,}5$$

</details>

**Exercice 5.** On sait que $$\lvert AB \rvert = \lvert A'B' \rvert$$, $$\lvert AC \rvert = \lvert A'C' \rvert$$ et $$\hat{A} = \hat{A}'$$. Les triangles sont-ils isométriques ? Par quel critère ?

<details>
<summary>Indice</summary>

Où se trouve l'angle $$\hat{A}$$ par rapport aux côtés $$[AB]$$ et $$[AC]$$ ?

</details>

<details>
<summary>Solution</summary>

- $$\hat{A}$$ est au sommet commun de $$[AB]$$ et $$[AC]$$ → c'est l'angle **entre** les 2 côtés
- ↳ critère **CAC** → $$\triangle ABC \cong \triangle A'B'C'$$

</details>

**Exercice 6 (TE F-1, octobre 2022, Ex. 1 i).** L'arc $$\widehat{ADC}$$ est un demi-cercle, $$\overline{AD} = \sqrt{21}$$ et $$\overline{DC} = 10$$. Calculer la hauteur $$h$$ du triangle $$ACD$$ (issue de $$D$$), avec deux chiffres après la virgule.

<details>
<summary>Indice</summary>

Demi-cercle → où est l'angle droit ? Calcule d'abord $$\overline{AC}$$, puis utilise les triangles semblables comme dans l'Ex 5 résolu.

</details>

<details>
<summary>Solution</summary>

- Demi-cercle → rectangle en $$D$$ → $$\overline{AC}^2 = 21 + 100 = 121$$ ↳ $$\overline{AC} = 11$$
- Triangles semblables (même angle en $$C$$, tous deux rectangles) : $$\frac{h}{\overline{DC}} = \frac{\overline{AD}}{\overline{AC}}$$
- $$h = \frac{\sqrt{21} \cdot 10}{11} \approx 4{,}17$$
- ↳ la correction du test trouve aussi $$4{,}17$$, mais en passant par $$h = \sqrt{21} \cdot \sin(\alpha)$$ (chapitre 3)

</details>

**Exercice 7 (TE F-1, octobre 2020, Ex. 1 a, partie triangle).** Triangle rectangle d'hypoténuse $$c = 2$$, un côté de l'angle droit $$b = \sqrt{3}$$. On trace la hauteur $$d$$ depuis l'angle droit sur l'hypoténuse. Donner $$a$$ et $$d$$ en valeurs **exactes** (pas de résultat machine).

<details>
<summary>Indice</summary>

$$a$$ : Pythagore. $$d$$ : le petit triangle formé par $$d$$ et $$b$$ est semblable au grand.

</details>

<details>
<summary>Solution</summary>

- $$a^2 = c^2 - b^2 = 4 - 3 = 1$$ ↳ $$a = 1$$
- Petit triangle (côtés $$d$$, `hyp` $$b$$) semblable au grand (côtés $$a$$, `hyp` $$c$$) : $$\frac{d}{b} = \frac{a}{c}$$
- $$d = \frac{a \cdot b}{c} = \frac{1 \cdot \sqrt{3}}{2} = \frac{\sqrt{3}}{2}$$
- ↳ réponses de la copie corrigée : $$a = 1$$, $$d = \frac{\sqrt{3}}{2}$$

</details>

**Exercice 8 (TE F-1, octobre 2020, Ex. 1 b).** Triangles semblables, dessins non proportionnels. Dans chaque grand triangle, un segment est **parallèle** à un côté.

1. Base totale $$8 + 2$$, côté $$10$$. Le segment $$x$$, parallèle au côté $$10$$, part du point situé à $$8$$ sur la base.
2. Base totale $$8 + 2$$, segment $$4$$ parallèle au côté $$y$$, partant du point situé à $$8$$.
3. Base totale $$4 + z$$, côté $$10$$, segment $$1$$ parallèle au côté $$10$$, partant du point situé à $$4$$.

<details>
<summary>Indice</summary>

Petit triangle / grand triangle : $$\frac{\text{segment}}{\text{côté parallèle}} = \frac{\text{petite base}}{\text{grande base}}$$.

</details>

<details>
<summary>Solution</summary>

- $$\frac{x}{10} = \frac{8}{10}$$ ↳ $$x = 8$$
- $$\frac{4}{y} = \frac{8}{10}$$ ↳ $$y = 5$$
- $$\frac{1}{10} = \frac{4}{4 + z}$$ ↳ $$4 + z = 40$$ ↳ $$z = 36$$
- ↳ ce sont les réponses validées sur la copie corrigée

</details>

**Exercice 9 (Janka, Test 1 Pb 2, 2023/24, partie angles, sans calculatrice).** Triangle rectangle en $$A$$ ; $$B$$ est sur $$[AC]$$. On donne $$\alpha = \angle ADB$$ et $$\beta = \angle ADC$$. Exprimer $$\angle ABD$$, $$\angle DBC$$, $$\angle BDC$$ et $$\angle BCD$$ en fonction de $$\alpha$$ et $$\beta$$.

<details>
<summary>Indice</summary>

Somme des angles dans $$\triangle ABD$$ puis $$\triangle ACD$$. Pour $$\angle DBC$$ : angles sur la droite $$(AC)$$.

</details>

<details>
<summary>Solution</summary>

- $$\triangle ABD$$ : $$\angle ABD = 180^\circ - 90^\circ - \alpha = 90^\circ - \alpha$$
- Sur la droite $$(AC)$$ : $$\angle DBC = 180^\circ - (90^\circ - \alpha) = 90^\circ + \alpha$$
- $$\angle BDC = \angle ADC - \angle ADB = \beta - \alpha$$
- $$\triangle ACD$$ : $$\angle BCD = 180^\circ - 90^\circ - \beta = 90^\circ - \beta$$
- Vérif dans $$\triangle BCD$$ : $$(90^\circ + \alpha) + (\beta - \alpha) + (90^\circ - \beta) = 180^\circ$$ ✓
- ↳ la suite de l'exercice (exprimer $$\lvert AB \rvert$$ et $$\lvert AD \rvert$$) utilise la loi des sinus → chapitre 4

</details>

> Source : Ex 6 : Algebre_merged.pdf, p. 223 ; Ex 7–8 : p. 214 ; Ex 9 : p. 250

## Liens avec les évaluations

**Ce chapitre tombe à chaque TE F-1**, en **Exercice 1** (6 à 8 points, environ 10 à 15 min) :

| Test | Exercice | Ce qui vient du chapitre 1 | Page |
| --- | --- | --- | --- |
| TE F-1 oct. 2020 | Ex. 1 « Angle & Co. » | Pythagore, hauteur, triangles semblables ($$x, y, z$$) | 214 |
| TE F-1 oct. 2022 | Ex. 1 « Triangle & Co. » | demi-cercle → angle droit, Pythagore, hauteur $$h$$ | 223 |
| TE F-1 nov. 2023 | Ex. 1 « Triangle & Co. » | idem (avec $$\overline{AD} = 25$$) | 232 |
| TE F-1 oct. 2025 | Ex. 1 « Triangle & Co. » | idem + distance $$\delta$$ entre $$B$$ et $$D$$ | 241 |
| Janka Test 1 Pb 2 (2023/24) | Question 1 | somme des angles, angles supplémentaires | 250 |
| Janka Test 1 Pb 2 (2024/25) | Question 1 « l'avion » | angles d'élévation dans des triangles rectangles (surtout chapitre 3) | 5, 53–60 |

**Démarche attendue** (d'après les corrections) :

1. **Repérer les triangles rectangles** (demi-cercle, hauteur) → c'est la clé de l'exercice
2. Pythagore pour le côté manquant, puis triangles semblables ou $$\sin$$ / $$\cos$$ pour $$h$$
3. Les angles restants → chapitres 3 à 5 (arcsin, loi des sinus). ⚠ Piège récurrent : arcsin donne un angle aigu, alors que l'angle cherché est obtus. En 2023, la correction barre « ≈ 60° » et écrit $$\pi - \beta$$. En 2025, la copie prend $$\beta = \pi - \beta_0 \approx 2{,}08$$ rad.
4. **Tout rédiger** : calculs explicites, deux chiffres après la virgule, angles en radians

**Tests de M. Janka** : 15 min, **sans calculatrice** → valeurs exactes, raisonnement sur les angles.

> Source : Algebre_merged.pdf, p. 5, 53–60, 214, 222 (consignes), 223, 232, 241, 250
