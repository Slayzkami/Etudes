---
aliases:
  - "Groupe abélien"
  - "abélien"
  - "commutatif"
  - "groupe commutatif"
tags:
  - gac
  - gac/definition
  - gac/chapitre-01
---

# 📘 Groupe abélien

*Définition* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.1 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Un [[groupe]] $(G,\star)$ est **abélien** (ou commutatif) si $\forall x,y\in G,\ x\star y=y\star x$.

> [!EXAMPLE] Exemples
> - Abéliens : $(\mathbb Z,+)$, $(\mathbb R^*,\times)$, $\mathbb U$, $\mathbb Z/n\mathbb Z$, Klein, tout [[groupe-monogene-cyclique|groupe monogène]].
> - Non abéliens : $\mathfrak S_n$ pour $n\ge3$, $GL_2(\mathbb R)$, $D_3$, $D_4$.

> [!WARNING] Vrai/Faux classique : « Tout groupe abélien est cyclique »
> **FAUX.** Contre-exemple : le groupe de Klein $K=\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z=\{(\bar0,\bar0),(\bar1,\bar0),(\bar0,\bar1),(\bar1,\bar1)\}$.
>
> **1. $K$ est abélien.** On additionne coordonnée par coordonnée, et $\mathbb Z/2\mathbb Z$ est abélien : pour tous $(a,b),(c,d)\in K$,
> $$(a,b)+(c,d)=(a+c,\ b+d)=(c+a,\ d+b)=(c,d)+(a,b).$$
>
> **2. $K$ n'est pas cyclique.** Supposons par l'absurde $K=\langle x\rangle$. Comme $o(x)=\mathrm{Card}\,\langle x\rangle$ ([[ordre-element]]), on aurait $o(x)=\mathrm{Card}\,K=4$.
> Or pour tout $x=(a,b)\in K$ : $2x=(2a,\ 2b)=(\bar0,\bar0)$, car $\bar2=\bar0$ dans $\mathbb Z/2\mathbb Z$.
> Donc $o(x)$ divise $2$ : $o(x)\in\{1,2\}$, et $\langle x\rangle$ a au plus $2$ éléments. Contradiction : $K\neq\langle x\rangle$ pour tout $x$.
>
> **Conclusion :** $K$ est abélien et non cyclique, donc l'affirmation est fausse.
>
> *En clair :* « cyclique » veut dire qu'un seul élément, ajouté à lui-même encore et encore, fabrique tout le groupe. Dans $\mathbb Z/4\mathbb Z$, $\bar1\to\bar2\to\bar3\to\bar0$ passe par les 4 éléments. Dans Klein, chaque élément revient à $(\bar0,\bar0)$ en 2 pas : $(\bar1,\bar0)\to(\bar0,\bar0)$. On n'atteint jamais les 4 éléments.

> [!TIP] La réciproque est vraie : tout groupe cyclique est abélien
> Si $G=\langle a\rangle$, deux éléments s'écrivent $a^k$ et $a^l$, et $a^ka^l=a^{k+l}=a^la^k$ ([[regles-de-calcul]]).

## 🔗 Liens

- **S'appuie sur** : [[groupe|Groupe]]
- **Utilisé par (définitions)** : [[centre|Centre d'un groupe]], [[sous-groupe-distingue|Sous-groupe distingué]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
