---
aliases:
  - "Méthode : montrer qu'une partie EST ouverte ou fermée"
  - "prouver ouvert"
  - "prouver fermé"
  - "image réciproque d'un ouvert"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : montrer qu'une partie EST ouverte ou fermée

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.1 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Par ordre de rapidité :
> 1. **Image réciproque** : écrire $A=f^{-1}(O)$ avec $f$ continue **sur tout l'espace** et $O$ ouvert (resp. $f^{-1}(\text{fermé})$). Inégalités **strictes** → ouvert ; **larges ou égalités** → fermé.
> 2. **Opérations** : réunion quelconque / intersection finie d'ouverts ; intersection quelconque / réunion **finie** de fermés.
> 3. **Fermé par les suites** : « soit $(x_n)$ une suite de $A$ qui converge vers $\ell\in E$ ; montrons $\ell\in A$ ».
> 4. **Ouvert par les boules** : pour $x\in A$, donner un rayon **explicite** $r>0$ avec $B(x,r)\subset A$.
> 5. **Fermé par le complémentaire** : montrer que $A^c$ est une réunion d'intervalles ouverts (utile dans $\mathbb R$).

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$X=\{(x,y)\mid x\ge0,\ y=x^2\}$ est fermé.* « Les applications $g(x,y)=y-x^2$ et $h(x,y)=x$ sont continues sur $\mathbb R^2$ (polynomiales). Donc $X=g^{-1}(\{0\})\cap h^{-1}([0,+\infty[)$ est une intersection de deux images réciproques de fermés par des applications continues : c'est un fermé. »
>
> *$\{f\neq g\}$ est ouvert ($f,g:E\to\mathbb R$ continues).* « $h=f-g$ est continue et $\{f\neq g\}=h^{-1}(\mathbb R\setminus\{0\})$, image réciproque d'un ouvert : c'est un ouvert. »
>
> *$\mathbb Z$ est fermé dans $\mathbb R$.* « $\mathbb R\setminus\mathbb Z=\bigcup_{n\in\mathbb Z}]n,n+1[$ est une réunion d'ouverts, donc un ouvert : $\mathbb Z$ est fermé. »

> [!WARNING] Pièges
> - Une réunion **infinie** de fermés n'est pas fermée en général : ne jamais écrire « réunion de fermés donc fermé » sans « finie ».
> - Définir $f$ sur $\mathbb R$ (ou $\mathbb R^2$), pas sur $A$ : écrire « $f:\mathbb R\to\mathbb R$, $f(x)=x$ » et non « $f:A\to\mathbb R$ » (mon erreur).
> - Toujours **conclure** : « donc $A$ est ouvert ».

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite-globale|Continuité globale : image réciproque]], [[topo-stabilite-ouverts|Stabilité des ouverts]], [[topo-stabilite-fermes|Stabilité des fermés]], [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]], [[topo-operations-fonctions-continues|Opérations sur les fonctions continues réelles]]
- **Méthodes voisines** : [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
- **Corrigés** : [[topo-exercices-types-corriges#4. Les ensembles {f = g} et {f ≠ g}|ex. 4]], [[topo-exercices-types-corriges#16. Ouverts et fermés de R²|ex. 16]]
- **Voir aussi** : [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
