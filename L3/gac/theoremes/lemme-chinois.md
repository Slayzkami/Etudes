---
aliases:
  - "Lemme chinois (groupes)"
  - "restes chinois"
  - "Z/mnZ ≃ Z/mZ × Z/nZ"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-03
---

# ⭐ Lemme chinois (groupes)

*Théorème* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.6 (ex. 1) du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $\operatorname{pgcd}(m_1,m_2)=1$ : $\mathbb Z/m_1m_2\mathbb Z\simeq\mathbb Z/m_1\mathbb Z\times\mathbb Z/m_2\mathbb Z$, via $\bar n\mapsto(n\bmod m_1,\ n\bmod m_2)$.

> [!SUCCESS]- Démonstration
> $\varphi:\mathbb Z\to\mathbb Z/m_1\mathbb Z\times\mathbb Z/m_2\mathbb Z$, $n\mapsto(n\bmod m_1, n\bmod m_2)$ est un morphisme.
> - Noyau : $m_1\mid n$ et $m_2\mid n$ ⟺ $m_1m_2\mid n$ (Gauss).
> - Surjectif : Bézout $um_1+vm_2=1$ ; $n=avm_2+bum_1$ s'envoie sur $(\bar a,\bar b)$.
> - [[premier-theoreme-isomorphisme]].

> [!WARNING] Hypothèse indispensable
> $\mathbb Z/4\mathbb Z\not\simeq\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ ; $\mathbb Z/8\mathbb Z\not\simeq\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z$.

## 🔗 Liens

- **S'appuie sur** : [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]], [[groupe-produit|Groupe produit]]
