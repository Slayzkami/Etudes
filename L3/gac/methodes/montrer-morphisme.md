---
aliases:
  - "Méthode : étudier un morphisme (morphisme, noyau, image, injectif, surjectif)"
  - "montrer qu'une application est un morphisme"
  - "étudier un morphisme"
  - "calculer le noyau"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : étudier un morphisme (morphisme, noyau, image, injectif, surjectif)

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette (toujours dans cet ordre)
> 0. **Si la source est un quotient** ($\mathbb Z/n\mathbb Z$, $G/H$) : d'abord montrer que $f$ est **bien définie** → [[morphisme-sur-quotient]].
> 1. **Morphisme** : « Soient $x,y\in G$. » Calculer $f(x\star y)$ et arriver à $f(x)\,\square\,f(y)$, en faisant attention à la loi de **chaque** groupe ($+$ au départ peut devenir $\times$ à l'arrivée).
> 2. **Noyau** : résoudre l'équation $f(x)=e'$ (le **neutre du groupe d'arrivée**). $\mathrm{Ker}\,f=\{x\in G\mid f(x)=e'\}$.
> 3. **Injectif ?** $f$ injectif $\iff\mathrm{Ker}\,f=\{e\}$ → [[noyau-et-image]].
> 4. **Image** : $\mathrm{Im}\,f=\{f(x),\ x\in G\}$. Surjectif $\iff\mathrm{Im}\,f=G'$ : prendre $y\in G'$ quelconque et **exhiber** un antécédent.
> 5. **Conclusion** : bijectif ⟹ isomorphisme ; sinon $G/\mathrm{Ker}\,f\simeq\mathrm{Im}\,f$ ([[premier-theoreme-isomorphisme]]).

> [!TIP] Ce qu'on a gratuitement
> $f(e)=e'$, $f(x^{-1})=f(x)^{-1}$, $f(x^n)=f(x)^n$ ([[proprietes-morphismes]]) ; $\mathrm{Ker}\,f$ est un sous-groupe **distingué**, $\mathrm{Im}\,f$ un sous-groupe.
> Si $G$ est fini : $\mathrm{Card}\,G=\mathrm{Card}(\mathrm{Ker}\,f)\times\mathrm{Card}(\mathrm{Im}\,f)$ (conséquence du 1er théorème d'isomorphisme et de [[lagrange]]) : pratique pour **contrôler** ses calculs.

> [!EXAMPLE] Rédaction modèle : $f:(\mathbb R,+)\to(\mathbb C^*,\times)$, $t\mapsto e^{2i\pi t}$
> - Soient $s,t\in\mathbb R$ : $f(s+t)=e^{2i\pi(s+t)}=e^{2i\pi s}e^{2i\pi t}=f(s)f(t)$. Morphisme.
> - $f(t)=1\iff 2\pi t\in2\pi\mathbb Z\iff t\in\mathbb Z$ : $\mathrm{Ker}\,f=\mathbb Z\neq\{0\}$, $f$ n'est pas injectif.
> - $|f(t)|=1$ donc $\mathrm{Im}\,f\subset\mathbb U$ ; et tout $z\in\mathbb U$ s'écrit $e^{i\theta}=f(\theta/2\pi)$ : $\mathrm{Im}\,f=\mathbb U$.
> - Conclusion : $\mathbb R/\mathbb Z\simeq\mathbb U$.

> [!WARNING] Pièges
> - Pour **réfuter** « $f$ est un morphisme » : un contre-exemple chiffré, ou $f(e)\neq e'$. Ex. : $x\mapsto x+1$ sur $(\mathbb Z,+)$ envoie $0$ sur $1$.
> - Le noyau se calcule avec le neutre **d'arrivée** : pour $\det:GL_n(\mathbb R)\to\mathbb R^*$, c'est $\det M=1$, pas $0$.

## 🔗 Liens

- **S'appuie sur** : [[morphisme-de-groupes|Morphisme de groupes]], [[image-noyau|Image, noyau]], [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]], [[proprietes-morphismes|Propriétés des morphismes]]
- **Voir aussi** : [[morphisme-sur-quotient]], [[identifier-quotient]], [[endomorphismes-de-z]]
- **Corrigés** : [[exercices-types-corriges#3. Morphisme Z/18Z → Z/6Z et quotient|ex. 3]], [[exercices-types-corriges#10. Étudier un morphisme|ex. 10]], [[exercices-types-corriges#18. Morphismes de Z/4Z dans Z/6Z|ex. 18]]
