---
aliases:
  - "Méthode : montrer que deux groupes ne sont pas isomorphes"
  - "pas isomorphes"
  - "invariants"
tags:
  - gac
  - gac/methode
  - gac/chapitre-01
---

# 🛠️ Méthode : montrer que deux groupes ne sont pas isomorphes

*Méthode* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Trouver une propriété **conservée par isomorphisme** que l'un a et pas l'autre :
> - le cardinal ; abélien ou non ; cyclique ou non ;
> - le nombre d'éléments d'ordre donné (un isomorphisme est injectif donc conserve l'ordre).

> [!EXAMPLE] Rédaction modèle : $\mathbb Z/4\mathbb Z\not\simeq\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$
> Dans Klein, $x+x=0$ pour tout $x$. Si $f:\mathbb Z/4\mathbb Z\to K$ était un isomorphisme, $f(\bar2)=f(\bar1)+f(\bar1)=0=f(\bar0)$, donc $\bar2=\bar0$ par injectivité : absurde.
> Autres : $\mathbb Z/18\mathbb Z\not\simeq\mathbb Z/6\mathbb Z$ (cardinaux 18 ≠ 6) ; $\mathfrak S_3\not\simeq\mathbb Z/6\mathbb Z$ (non abélien).

## 🔗 Liens

- **Utilisé par (définitions)** : [[groupes-isomorphes|Groupes isomorphes]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
- **Voir aussi** : [[ordre-element|Ordre d'un élément]]
