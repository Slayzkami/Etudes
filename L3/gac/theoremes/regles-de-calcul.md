---
aliases:
  - "Règles de calcul dans un groupe"
  - "(ab)^-1"
  - "simplification"
  - "régulier"
  - "résolution d'équations"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-01
---

# ⭐ Règles de calcul dans un groupe

*Théorème* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.2 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Pour $a,b,c$ dans un [[groupe]] multiplicatif :
> 1. $1^{-1}=1$, $(a^{-1})^{-1}=a$, $(ab)^{-1}=b^{-1}a^{-1}$ ;
> 2. $\forall m,n\in\mathbb Z$ : $a^na^m=a^{n+m}$, $(a^n)^m=a^{nm}$, $(a^n)^{-1}=a^{-n}$ ;
> 3. **simplification** : $ac=bc\Rightarrow a=b$ et $ca=cb\Rightarrow a=b$ ;
> 4. **équations** : $ax=b\iff x=a^{-1}b$ ; $xa=b\iff x=ba^{-1}$ ;
> 5. si $ab=ba$ : $(ab)^n=a^nb^n$.

> [!SUCCESS]- Démonstration (points clés)
> - $(ab)(b^{-1}a^{-1})=a(bb^{-1})a^{-1}=1$ et de même à gauche ; unicité de l'inverse.
> - Simplifier : multiplier à droite (ou à gauche) par $c^{-1}$.
> - Conséquence : dans un groupe, $x^2=x\Rightarrow x=1$ (simplifier par $x$).

> [!WARNING] Pièges
> - $(ab)^{-1}\neq a^{-1}b^{-1}$ en général (chaussette/chaussure).
> - Si $(xy)^2=x^2y^2$ pour tous $x,y$, alors $G$ est abélien (simplifier $xyxy=xxyy$) (TD1 ex. 2).
> - Si $x^2=1$ pour tout $x$, alors $G$ est abélien : $xy=(xy)^{-1}=y^{-1}x^{-1}=yx$ (TD1 ex. 14).

## 🔗 Liens

- **S'appuie sur** : [[groupe|Groupe]], [[puissances-multiples|Puissances et multiples]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
