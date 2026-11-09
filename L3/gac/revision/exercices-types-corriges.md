---
aliases:
  - "Exercices types corrigés"
  - "corrections modèles"
  - "exercices du partiel"
tags:
  - gac
  - gac/revision
---

# ✍️ Exercices types corrigés (rédactions modèles)

Les exercices qui reviennent dans les sujets, rédigés comme sur une copie. **Mode d'emploi** : lire l'énoncé, chercher sur brouillon, puis seulement déplier la correction et comparer ligne par ligne. · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]]

> [!NOTE] Sommaire
> 1. [[#1. Ordres et sous-groupes de Z/18Z]]
> 2. [[#2. Réunion de deux sous-groupes]]
> 3. [[#3. Morphisme Z/18Z → Z/6Z et quotient]]
> 4. [[#4. Loi exotique a ⋆ b = a + b + ab]]
> 5. [[#5. Endomorphismes de (Z, +)]]
> 6. [[#6. Relation d'équivalence associée à une application]]
> 7. [[#7. Montrer qu'une partie est un sous-groupe]]
> 8. [[#8. Identifier un quotient]]
> 9. [[#9. Groupe d'ordre premier]]
> 10. [[#10. Étudier un morphisme]]
> 11. [[#11. Ordres dans un produit]]
> 12. [[#12. Classes, indice et quotient]]
> 13. [[#13. Centre et sous-groupe distingué]]
> 14. [[#14. Sous-groupes de S3]]
> 15. [[#15. Groupe où tout élément vérifie x² = e]]
> 16. [[#16. Automorphismes intérieurs]]
> 17. [[#17. Ordre de l'inverse et d'un conjugué]]
> 18. [[#18. Morphismes de Z/4Z dans Z/6Z]]
> 19. [[#19. Intersection et somme de sous-groupes de Z]]
>
> Pour savoir quelle méthode sortir face à un énoncé : [[reconnaitre-exercice]].

---

## 1. Ordres et sous-groupes de Z/18Z

**Énoncé.** Dans $(\mathbb Z/18\mathbb Z,+)$ :
a) calculer l'ordre de $\overline{12}$ et de $\overline{15}$ ;
b) déterminer $\langle\overline{12}\rangle$ et $\langle\bar6\rangle$, et les comparer ;
c) donner tous les générateurs de $\mathbb Z/18\mathbb Z$ ;
d) donner tous les sous-groupes de $\mathbb Z/18\mathbb Z$ et le diagramme des inclusions.

Méthodes : [[calculer-dans-znz]], [[calculer-ordre]], [[lister-sous-groupes-znz]].

> [!SUCCESS]- Correction a)
> D'après le cours, $o(\bar k)=\dfrac{18}{\operatorname{pgcd}(18,k)}$ ([[ordre-dans-znz]]).
> - $\operatorname{pgcd}(18,12)=6$, donc $o(\overline{12})=18/6=3$.
>   Vérification : $1\cdot\overline{12}=\overline{12}\neq\bar0$, $2\cdot\overline{12}=\overline{24}=\bar6\neq\bar0$, $3\cdot\overline{12}=\overline{36}=\bar0$.
> - $\operatorname{pgcd}(18,15)=3$, donc $o(\overline{15})=18/3=6$.

> [!SUCCESS]- Correction b)
> $\langle\overline{12}\rangle=\{k\cdot\overline{12},\ k\in\mathbb Z\}$. Comme $o(\overline{12})=3$, il a 3 éléments : $\langle\overline{12}\rangle=\{\bar0,\overline{12},\bar6\}$.
> De même $1\cdot\bar6=\bar6$, $2\cdot\bar6=\overline{12}$, $3\cdot\bar6=\overline{18}=\bar0$ : $\langle\bar6\rangle=\{\bar0,\bar6,\overline{12}\}$.
> Donc **$\langle\bar6\rangle=\langle\overline{12}\rangle$** : deux éléments différents peuvent engendrer le même sous-groupe.

> [!SUCCESS]- Correction c)
> $\bar k$ engendre $\mathbb Z/18\mathbb Z$ ssi $o(\bar k)=18$, ssi $\operatorname{pgcd}(18,k)=1$.
> Les générateurs sont donc $\bar1,\bar5,\bar7,\overline{11},\overline{13},\overline{17}$.

> [!SUCCESS]- Correction d)
> Les sous-groupes de $\mathbb Z/18\mathbb Z$ sont les $\langle\bar d\rangle$ pour $d$ diviseur positif de $18$, et $\langle\bar d\rangle$ a $18/d$ éléments.
>
> | $d$ | sous-groupe | ordre |
> |---|---|---|
> | 1 | $\langle\bar1\rangle=\mathbb Z/18\mathbb Z$ | 18 |
> | 2 | $\langle\bar2\rangle=\{\bar0,\bar2,\bar4,\dots,\overline{16}\}$ | 9 |
> | 3 | $\langle\bar3\rangle=\{\bar0,\bar3,\bar6,\bar9,\overline{12},\overline{15}\}$ | 6 |
> | 6 | $\langle\bar6\rangle=\{\bar0,\bar6,\overline{12}\}$ | 3 |
> | 9 | $\langle\bar9\rangle=\{\bar0,\bar9\}$ | 2 |
> | 18 | $\langle\overline{18}\rangle=\{\bar0\}$ | 1 |
>
> Inclusions : $\langle\bar a\rangle\subset\langle\bar b\rangle\iff b\mid a$.
>
> ```mermaid
> graph BT
>   Z0["{0}"] --> Z9["⟨9⟩ (ordre 2)"]
>   Z0 --> Z6["⟨6⟩ (ordre 3)"]
>   Z9 --> Z3["⟨3⟩ (ordre 6)"]
>   Z6 --> Z3
>   Z6 --> Z2["⟨2⟩ (ordre 9)"]
>   Z3 --> Z1["Z/18Z (ordre 18)"]
>   Z2 --> Z1
> ```

---

## 2. Réunion de deux sous-groupes

**Énoncé.** Donner deux sous-groupes $H$ et $K$ de $\mathbb Z/18\mathbb Z$ tels que $H\cup K$ ne soit pas un sous-groupe.

> [!SUCCESS]- Correction
> Prenons $H=\langle\bar9\rangle=\{\bar0,\bar9\}$ et $K=\langle\bar6\rangle=\{\bar0,\bar6,\overline{12}\}$.
> Alors $H\cup K=\{\bar0,\bar6,\bar9,\overline{12}\}$.
> Or $\bar6\in H\cup K$ et $\bar9\in H\cup K$, mais $\bar6+\bar9=\overline{15}\notin H\cup K$.
> Donc $H\cup K$ n'est pas stable par $+$ : ce n'est pas un sous-groupe.
> (Autre argument : $H\cup K$ a 4 éléments et $4\nmid18$, impossible d'après [[lagrange]].)
> → [[intersection-sous-groupes]]

---

## 3. Morphisme Z/18Z → Z/6Z et quotient

**Énoncé.** Soit $f:\mathbb Z/18\mathbb Z\to\mathbb Z/6\mathbb Z$, $x+18\mathbb Z\mapsto x+6\mathbb Z$.
a) Montrer que $f$ est bien définie. 
b) Montrer que $f$ est un morphisme de groupes. 
c) Déterminer $\mathrm{Ker}\,f$ et $\mathrm{Im}\,f$. 
d) En déduire un isomorphisme. 
e) $\mathbb Z/6\mathbb Z$ est-il un sous-groupe de $\mathbb Z/18\mathbb Z$ ? Les deux groupes sont-ils isomorphes ?

Méthode : [[morphisme-sur-quotient]].

> [!SUCCESS]- Correction a) bien définie
> Il faut montrer que le résultat ne dépend pas du représentant choisi.
> Soient $x,y\in\mathbb Z$ tels que $x+18\mathbb Z=y+18\mathbb Z$. Alors $18\mid x-y$. Comme $6\mid18$, on a $6\mid x-y$, donc $x+6\mathbb Z=y+6\mathbb Z$.
> Donc $f$ est bien définie.

> [!SUCCESS]- Correction b) morphisme
> Soient $x,y\in\mathbb Z$.
> $f\big((x+18\mathbb Z)+(y+18\mathbb Z)\big)=f\big((x+y)+18\mathbb Z\big)=(x+y)+6\mathbb Z=(x+6\mathbb Z)+(y+6\mathbb Z)=f(x+18\mathbb Z)+f(y+18\mathbb Z)$.
> Donc $f$ est un morphisme de groupes.

> [!SUCCESS]- Correction c) noyau et image
> $x+18\mathbb Z\in\mathrm{Ker}\,f\iff x+6\mathbb Z=6\mathbb Z\iff 6\mid x$.
> Donc $\mathrm{Ker}\,f=\{\bar0,\bar6,\overline{12}\}=\langle\bar6\rangle=6\mathbb Z/18\mathbb Z$.
> Pour tout $k\in\mathbb Z$, $k+6\mathbb Z=f(k+18\mathbb Z)$ : $f$ est surjective, $\mathrm{Im}\,f=\mathbb Z/6\mathbb Z$.
> ($f$ n'est pas injective car $\mathrm{Ker}\,f\neq\{\bar0\}$.)

> [!SUCCESS]- Correction d) isomorphisme
> D'après le [[premier-theoreme-isomorphisme|premier théorème d'isomorphisme]], $(\mathbb Z/18\mathbb Z)/\mathrm{Ker}\,f\simeq\mathrm{Im}\,f$, c'est-à-dire
> $$(\mathbb Z/18\mathbb Z)\big/(6\mathbb Z/18\mathbb Z)\simeq\mathbb Z/6\mathbb Z.$$
> Contrôle des cardinaux : $18/3=6$ ✔.

> [!SUCCESS]- Correction e)
> - $\mathbb Z/6\mathbb Z$ n'est pas une **partie** de $\mathbb Z/18\mathbb Z$ (ses éléments sont des classes modulo 6, pas modulo 18), donc ce n'est pas un sous-groupe. En revanche $\langle\bar3\rangle\le\mathbb Z/18\mathbb Z$ est cyclique d'ordre 6, donc isomorphe à $\mathbb Z/6\mathbb Z$ ([[structure-groupes-monogenes]]).
> - Ils ne sont pas isomorphes : un isomorphisme est une bijection, or $18\neq6$ ([[montrer-non-isomorphes]]).

---

## 4. Loi exotique a ⋆ b = a + b + ab

**Énoncé.** Sur $G=\mathbb R\setminus\{-1\}$ on pose $a\star b=a+b+ab$. Montrer que $(G,\star)$ est un groupe abélien.

Méthode : [[montrer-groupe]]. **L'astuce à voir** : $1+a\star b=(1+a)(1+b)$.

> [!SUCCESS]- Correction
> **Loi interne.** Soient $a,b\in G$. On a $1+a\star b=1+a+b+ab=(1+a)(1+b)$. Comme $a\neq-1$ et $b\neq-1$, ce produit est non nul, donc $a\star b\neq-1$ : $a\star b\in G$.
>
> **Associativité.** Soient $a,b,c\in G$. D'après la formule précédente,
> $1+(a\star b)\star c=(1+a\star b)(1+c)=(1+a)(1+b)(1+c)$ et $1+a\star(b\star c)=(1+a)(1+b\star c)=(1+a)(1+b)(1+c)$.
> Donc $(a\star b)\star c=a\star(b\star c)$.
>
> **Neutre.** $0\in G$ et pour tout $a\in G$ : $a\star0=a+0+0=a$ et $0\star a=a$. Le neutre est $0$.
>
> **Symétrique.** Soit $a\in G$. On cherche $b$ tel que $a+b+ab=0$, soit $b(1+a)=-a$, soit $b=\dfrac{-a}{1+a}$ (possible car $a\neq-1$).
> $b\in G$ : sinon $-a=-(1+a)$, soit $0=-1$, absurde. Et $a\star b=b\star a=0$ (la loi est commutative, voir ci-dessous).
>
> **Commutativité.** $a\star b=a+b+ab=b+a+ba=b\star a$.
>
> Donc $(G,\star)$ est un groupe abélien.
>
> **Bonus (isomorphisme).** $\varphi:G\to\mathbb R^*$, $a\mapsto1+a$ est une bijection et $\varphi(a\star b)=\varphi(a)\varphi(b)$ : c'est un isomorphisme de $(G,\star)$ sur $(\mathbb R^*,\times)$.

---

## 5. Endomorphismes de (Z, +)

**Énoncé.** Déterminer tous les morphismes de groupes $f:(\mathbb Z,+)\to(\mathbb Z,+)$. Lesquels sont des automorphismes ?

Méthode : [[endomorphismes-de-z]].

> [!SUCCESS]- Correction
> **Analyse.** Soit $f$ un endomorphisme de $(\mathbb Z,+)$ ; posons $a=f(1)\in\mathbb Z$. Pour tout $n\in\mathbb Z$, $f(n)=f(n\cdot1)=n\,f(1)=an$ ([[proprietes-morphismes]] : $f(nx)=nf(x)$).
>
> **Synthèse.** Réciproquement, pour $a\in\mathbb Z$, l'application $f_a:n\mapsto an$ vérifie $f_a(n+m)=a(n+m)=an+am=f_a(n)+f_a(m)$ : c'est un morphisme.
>
> **Conclusion.** Les endomorphismes de $(\mathbb Z,+)$ sont exactement les $f_a:n\mapsto an$, $a\in\mathbb Z$.
>
> **Automorphismes.** $\mathrm{Im}\,f_a=a\mathbb Z$, donc $f_a$ surjective $\iff a\mathbb Z=\mathbb Z\iff a=\pm1$ ; et $f_1=\mathrm{id}$, $f_{-1}=-\mathrm{id}$ sont bien bijectives. Donc $\mathrm{Aut}(\mathbb Z)=\{\mathrm{id},-\mathrm{id}\}$.
> (Pour $a\neq0$ : $\mathrm{Ker}\,f_a=\{0\}$, donc $f_a$ est injective ; $f_0$ est le morphisme nul.)

---

## 6. Relation d'équivalence associée à une application

**Énoncé.** Soit $f:E\to F$. On définit sur $E$ : $x\,\mathcal R\,y\iff f(x)=f(y)$. Montrer que $\mathcal R$ est une relation d'équivalence et décrire la classe de $x$.

> [!SUCCESS]- Correction
> - **Réflexive** : pour tout $x\in E$, $f(x)=f(x)$, donc $x\mathcal Rx$.
> - **Symétrique** : si $x\mathcal Ry$, alors $f(x)=f(y)$, donc $f(y)=f(x)$, donc $y\mathcal Rx$.
> - **Transitive** : si $x\mathcal Ry$ et $y\mathcal Rz$, alors $f(x)=f(y)=f(z)$, donc $x\mathcal Rz$.
>
> Donc $\mathcal R$ est une [[relation-equivalence|relation d'équivalence]]. La classe de $x$ est $\bar x=\{y\in E\mid f(y)=f(x)\}=f^{-1}(\{f(x)\})$.
> Exemple : $E=\mathbb C^*$, $f(z)=|z|$ : la classe de $z$ est le cercle de centre $0$ et de rayon $|z|$.

---

## 7. Montrer qu'une partie est un sous-groupe

**Énoncé.** Montrer que $\mathbb U_n=\{z\in\mathbb C^*\mid z^n=1\}$ est un sous-groupe de $(\mathbb C^*,\times)$.

Méthode : [[montrer-sous-groupe]].

> [!SUCCESS]- Correction (caractérisation)
> - $\mathbb U_n\subset\mathbb C^*$ et $1^n=1$, donc $1\in\mathbb U_n$.
> - Soient $x,y\in\mathbb U_n$. Alors $(xy^{-1})^n=x^n(y^n)^{-1}=1\cdot1^{-1}=1$ (car $\mathbb C^*$ est abélien), donc $xy^{-1}\in\mathbb U_n$.
>
> D'après la [[caracterisation-sous-groupe|caractérisation des sous-groupes]], $\mathbb U_n\le\mathbb C^*$.

> [!SUCCESS]- Correction (variante express)
> $\varphi:\mathbb C^*\to\mathbb C^*$, $z\mapsto z^n$ est un morphisme ($(zz')^n=z^nz'^n$) et $\mathbb U_n=\mathrm{Ker}\,\varphi$ : c'est un sous-groupe ([[noyau-et-image]]).

---

## 8. Identifier un quotient

**Énoncé.** Montrer que $\mathbb R^*/\{-1,1\}\simeq\mathbb R_+^*$.

Méthode : [[identifier-quotient]].

> [!SUCCESS]- Correction
> Soit $f:(\mathbb R^*,\times)\to(\mathbb R_+^*,\times)$, $x\mapsto|x|$.
> - **Morphisme** : $|xy|=|x|\,|y|$.
> - **Noyau** : $|x|=1\iff x=\pm1$, donc $\mathrm{Ker}\,f=\{-1,1\}$.
> - **Image** : pour $y>0$, $y=|y|=f(y)$ : $f$ est surjective.
>
> D'après le [[premier-theoreme-isomorphisme|premier théorème d'isomorphisme]], $\mathbb R^*/\{-1,1\}\simeq\mathbb R_+^*$.

---

## 9. Groupe d'ordre premier

**Énoncé.** Soit $G$ un groupe d'ordre $p$ premier. Montrer que $G$ est cyclique.

> [!SUCCESS]- Correction
> Comme $p\ge2$, il existe $x\in G$, $x\neq1$. Le sous-groupe $\langle x\rangle$ a un ordre qui divise $p$ ([[lagrange]]), donc égal à $1$ ou $p$. Comme $x\neq1$, $\langle x\rangle\neq\{1\}$, donc $\mathrm{Card}\,\langle x\rangle=p=\mathrm{Card}\,G$, d'où $\langle x\rangle=G$.
> Donc $G$ est cyclique (et $G\simeq\mathbb Z/p\mathbb Z$, [[structure-groupes-monogenes]]). → [[groupe-ordre-premier]]
---

## 10. Étudier un morphisme

**Énoncé.** Soit $f:(\mathbb C^*,\times)\to(\mathbb C^*,\times)$, $z\mapsto z/|z|$. Montrer que $f$ est un morphisme, déterminer son noyau et son image, et en déduire un isomorphisme.

Méthode : [[montrer-morphisme]].

> [!SUCCESS]- Correction
> - **Morphisme.** Soient $z,z'\in\mathbb C^*$ : $f(zz')=\dfrac{zz'}{|zz'|}=\dfrac{z}{|z|}\cdot\dfrac{z'}{|z'|}=f(z)f(z')$.
> - **Noyau.** $f(z)=1\iff z=|z|\iff z\in\mathbb R_+^*$. Donc $\mathrm{Ker}\,f=\mathbb R_+^*$ ; $f$ n'est pas injectif.
> - **Image.** $|f(z)|=1$, donc $\mathrm{Im}\,f\subset\mathbb U$. Réciproquement, si $u\in\mathbb U$, $f(u)=u/1=u$. Donc $\mathrm{Im}\,f=\mathbb U$.
> - **Conclusion.** Par le [[premier-theoreme-isomorphisme|premier théorème d'isomorphisme]] : $\mathbb C^*/\mathbb R_+^*\simeq\mathbb U$.

---

## 11. Ordres dans un produit

**Énoncé.** Soit $G=\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z$. 
a) Donner l'ordre de chaque élément. 
b) $G$ est-il cyclique ? Est-il isomorphe à $\mathbb Z/8\mathbb Z$ ?

Méthodes : [[calculer-ordre]], [[montrer-cyclique]], [[montrer-non-isomorphes]].

> [!SUCCESS]- Correction
> a) $o(a,b)=\operatorname{ppcm}(o(a),o(b))$. Dans $\mathbb Z/2\mathbb Z$ : $o(\bar0)=1$, $o(\bar1)=2$. Dans $\mathbb Z/4\mathbb Z$ : $o(\bar0)=1$, $o(\bar1)=o(\bar3)=4$, $o(\bar2)=2$.
>
> | élément | $(\bar0,\bar0)$ | $(\bar0,\bar1)$ | $(\bar0,\bar2)$ | $(\bar0,\bar3)$ | $(\bar1,\bar0)$ | $(\bar1,\bar1)$ | $(\bar1,\bar2)$ | $(\bar1,\bar3)$ |
> |---|---|---|---|---|---|---|---|---|
> | ordre | 1 | 4 | 2 | 4 | 2 | 4 | 2 | 4 |
>
> b) $G$ a 8 éléments et aucun n'est d'ordre 8 : $G$ n'est pas cyclique. $\mathbb Z/8\mathbb Z$ est cyclique ($o(\bar1)=8$) ; un isomorphisme conserve l'ordre des éléments, donc $G\not\simeq\mathbb Z/8\mathbb Z$.

---

## 12. Classes, indice et quotient

**Énoncé.** Dans $G=\mathbb Z/12\mathbb Z$, soit $H=\langle\bar4\rangle$. 
a) Donner $H$ et son indice. 
b) Écrire toutes les classes modulo $H$. 
c) À quel groupe connu $G/H$ est-il isomorphe ?

Méthode : [[classes-et-indice]].

> [!SUCCESS]- Correction
> a) $H=\{\bar0,\bar4,\bar8\}$, $[H]=3$, $[G:H]=12/3=4$.
> b) $H=\{\bar0,\bar4,\bar8\}$, $\bar1+H=\{\bar1,\bar5,\bar9\}$, $\bar2+H=\{\bar2,\bar6,\overline{10}\}$, $\bar3+H=\{\bar3,\bar7,\overline{11}\}$.
> c) $G$ est abélien, donc $H\lhd G$ et $G/H$ est un groupe d'ordre 4.
> **Avec un morphisme** : $f:\mathbb Z/12\mathbb Z\to\mathbb Z/4\mathbb Z$, $x+12\mathbb Z\mapsto x+4\mathbb Z$ est bien définie (car $4\mid12$), c'est un morphisme surjectif, et $\mathrm{Ker}\,f=\{\bar x\mid4\mid x\}=H$. Donc $G/H\simeq\mathbb Z/4\mathbb Z$.

---

## 13. Centre et sous-groupe distingué

**Énoncé.** Soit $G$ un groupe et $Z(G)=\{z\in G\mid\forall g\in G,\ zg=gz\}$. Montrer que $Z(G)$ est un sous-groupe distingué de $G$.

Méthodes : [[montrer-sous-groupe]], [[montrer-distingue]].

> [!SUCCESS]- Correction
> **Sous-groupe.**
> - $e\in Z(G)$ car $eg=g=ge$ pour tout $g$.
> - Soient $x,y\in Z(G)$ et $g\in G$. De $yg=gy$ on tire, en multipliant à gauche et à droite par $y^{-1}$ : $gy^{-1}=y^{-1}g$. Alors $(xy^{-1})g=x(y^{-1}g)=x(gy^{-1})=(xg)y^{-1}=g(xy^{-1})$. Donc $xy^{-1}\in Z(G)$.
>
> **Distingué.** Soient $g\in G$ et $z\in Z(G)$ : $g^{-1}zg=g^{-1}gz=z\in Z(G)$.
>
> Donc $Z(G)\lhd G$. → [[centre]]

---

## 14. Sous-groupes de S3

**Énoncé.** Dans $\mathfrak S_3=\{e,\gamma,\gamma^2,\tau_1,\tau_2,\tau_3\}$ ($\gamma=(1\,2\,3)$, $\tau_1=(1\,2)$, $\tau_2=(1\,3)$, $\tau_3=(2\,3)$) : a) donner l'ordre de chaque élément ; b) donner tous les sous-groupes ; c) lesquels sont distingués ?

Méthodes : [[utiliser-lagrange]], [[montrer-distingue]].

> [!SUCCESS]- Correction
> a) $o(e)=1$ ; $o(\tau_i)=2$ (car $\tau_i\neq e$ et $\tau_i^2=e$) ; $o(\gamma)=o(\gamma^2)=3$.
> b) Par [[lagrange]], un sous-groupe est d'ordre 1, 2, 3 ou 6.
> - ordre 1 : $\{e\}$ ; ordre 6 : $\mathfrak S_3$ ;
> - ordre 2 (premier, donc engendré par un élément d'ordre 2) : $\{e,\tau_1\}$, $\{e,\tau_2\}$, $\{e,\tau_3\}$ ;
> - ordre 3 (premier, donc engendré par un élément d'ordre 3) : $\{e,\gamma,\gamma^2\}$.
>
> Soit 6 sous-groupes.
> c) $\{e\}$ et $\mathfrak S_3$ sont distingués. $\{e,\gamma,\gamma^2\}$ est d'indice $6/3=2$, donc distingué ([[indice-2-distingue]]).
> $\{e,\tau_1\}$ ne l'est pas : $\tau_2^{-1}\tau_1\tau_2=\tau_2\tau_1\tau_2=\tau_3\notin\{e,\tau_1\}$. De même pour $\{e,\tau_2\}$ et $\{e,\tau_3\}$.

---

## 15. Groupe où tout élément vérifie x² = e

**Énoncé.** Soit $G$ un groupe tel que $x^2=e$ pour tout $x\in G$. Montrer que $G$ est abélien.

> [!SUCCESS]- Correction
> Pour tout $x\in G$, $x\cdot x=e$ donc $x^{-1}=x$.
> Soient $x,y\in G$. Alors $xy=(xy)^{-1}=y^{-1}x^{-1}=yx$ ([[regles-de-calcul]]).
> Donc $G$ est abélien.

---

## 16. Automorphismes intérieurs

**Énoncé.** Soit $G$ un groupe et $a\in G$. Montrer que $f_a:G\to G$, $x\mapsto axa^{-1}$ est un automorphisme de $G$.

Méthode : [[montrer-morphisme]].

> [!SUCCESS]- Correction
> - **Morphisme.** Soient $x,y\in G$ : $f_a(x)f_a(y)=axa^{-1}aya^{-1}=axya^{-1}=f_a(xy)$.
> - **Bijectif.** Pour tout $x$ : $f_{a^{-1}}(f_a(x))=a^{-1}(axa^{-1})a=x$ et de même $f_a(f_{a^{-1}}(x))=x$. Donc $f_a$ est bijective, de réciproque $f_{a^{-1}}$.
>
> Donc $f_a\in\mathrm{Aut}\,G$. → [[automorphismes]]

---

## 17. Ordre de l'inverse et d'un conjugué

**Énoncé.** Soit $G$ un groupe, $x,y\in G$ avec $x$ d'ordre fini. Montrer que $o(x^{-1})=o(x)$ et $o(yxy^{-1})=o(x)$.

> [!SUCCESS]- Correction
> Soit $m\ge1$.
> - $(x^{-1})^m=(x^m)^{-1}$, donc $(x^{-1})^m=e\iff x^m=e$.
> - $(yxy^{-1})^m=yx^my^{-1}$ (les $y^{-1}y$ se simplifient), donc $(yxy^{-1})^m=e\iff x^m=y^{-1}y=e$.
>
> Dans les deux cas, les entiers $m\ge1$ qui conviennent sont les mêmes que pour $x$ ; le plus petit aussi. D'où l'égalité des ordres. → [[ordre-element]]

---

## 18. Morphismes de Z/4Z dans Z/6Z

**Énoncé.** Déterminer tous les morphismes de groupes $f:\mathbb Z/4\mathbb Z\to\mathbb Z/6\mathbb Z$.

Méthodes : [[endomorphismes-de-z]], [[morphisme-sur-quotient]].

> [!SUCCESS]- Correction
> **Analyse.** Soit $f$ un tel morphisme et $a=f(\bar1)$. Pour $x\in\mathbb Z$ : $f(\bar x)=f(x\cdot\bar1)=x\,a$ : $f$ est déterminé par $a$. De plus $4a=f(4\cdot\bar1)=f(\bar0)=\bar0$ dans $\mathbb Z/6\mathbb Z$.
> On teste : $4\cdot\bar0=\bar0$ ✔, $4\cdot\bar1=\bar4$, $4\cdot\bar2=\bar2$, $4\cdot\bar3=\overline{12}=\bar0$ ✔, $4\cdot\bar4=\bar4$, $4\cdot\bar5=\bar2$. Donc $a\in\{\bar0,\bar3\}$.
>
> **Synthèse.** Soit $a\in\{\bar0,\bar3\}$ et $f_a:\bar x\mapsto x\,a$.
> - Bien définie : si $\bar x=\bar y$ dans $\mathbb Z/4\mathbb Z$, $x-y=4k$, donc $xa-ya=k(4a)=\bar0$.
> - Morphisme : $f_a(\bar x+\bar y)=(x+y)a=xa+ya$.
>
> **Conclusion.** Il y a exactement deux morphismes : le morphisme nul et $\bar x\mapsto x\cdot\bar3$.

---

## 19. Intersection et somme de sous-groupes de Z

**Énoncé.** Déterminer $4\mathbb Z\cap6\mathbb Z$ et le sous-groupe $\langle4,6\rangle$ de $(\mathbb Z,+)$.

> [!SUCCESS]- Correction
> - $n\in4\mathbb Z\cap6\mathbb Z\iff4\mid n\text{ et }6\mid n\iff\operatorname{ppcm}(4,6)=12\mid n$. Donc $4\mathbb Z\cap6\mathbb Z=12\mathbb Z$.
> - **Inclusion $\supset$** : $2=6-4\in\langle4,6\rangle$, et $\langle4,6\rangle$ est un sous-groupe, donc il contient tous les multiples de $2$ : $2\mathbb Z\subset\langle4,6\rangle$.
> - **Inclusion $\subset$** : $2\mathbb Z$ est un sous-groupe de $\mathbb Z$ qui contient $4$ et $6$ ; or $\langle4,6\rangle$ est le **plus petit** sous-groupe contenant $4$ et $6$ : $\langle4,6\rangle\subset2\mathbb Z$.
> - Donc $\langle4,6\rangle=2\mathbb Z=\operatorname{pgcd}(4,6)\,\mathbb Z$.
>
> → [[sous-groupe-engendre]], [[intersection-sous-groupes]]

## 🔗 Liens

- Vrai/Faux rédigés : [[vrai-faux-classiques]]
- Encore plus d'exercices : [correction du TD1](../fichiers/gac-td1-correction.pdf), [sujet 2025](../fichiers/gac-sujet-2025-seconde-session.pdf)
- [[reconnaitre-exercice]] · [[mes-erreurs]] · [[fiche-definitions]] · [[fiche-theoremes]]
