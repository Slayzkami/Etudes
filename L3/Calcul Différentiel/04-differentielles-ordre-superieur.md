---
aliases:
  - "4 – Différentielles d'ordre supérieur"
  - "Chapitre hessienne extrema Taylor"
  - "CD chapitre 4"
tags:
  - cd
  - cd/chapitre
---

# Chapitre 04 – Différentielles d'ordre supérieur

**Matière :** [[L3/Calcul Différentiel/README|Calcul Différentiel]]  
**Source :** cours rédigé, chapitre 4 (pages 73 à 98)  
**Index :** [[cd-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- $D^2f_a$ est une application **bilinéaire symétrique** ([[theoreme-de-schwarz]]) ; sur $\mathbb R^n$, $D^2f_a(h,k)={}^t\!h\,H_f(a)\,k$ ([[matrice-hessienne]]).
- **Taylor-Young** : $f(a+h)=f(a)+Df_a(h)+\frac12{}^t\!h\,H_f(a)\,h+\lVert h\rVert^2\varepsilon(h)$ ([[taylor-young-ordre-2]]).
- **Extrema** : extremum local ⟹ point critique ; puis en dimension 2 le signe de $rt-s^2$ ([[critere-rt-s2]]).

## 📝 Notes

### 4.1 – Différentielle seconde
- [[differentielle-seconde]] : $D^2f_a=D(Df)_a$, vue comme bilinéaire ; [[theoreme-de-schwarz]].

### 4.2 – Dimension finie
- [[derivees-partielles-ordre-2]], [[expression-differentielle-seconde]], [[critere-c2]], [[matrice-hessienne]], [[taylor-young-ordre-2]].
- Méthodes : [[calculer-differentielle-seconde]], [[ecrire-taylor-young]].

### 4.3 – Extrema locaux
- [[extremum-local]], [[point-critique]], [[condition-necessaire-extremum]], [[extrema-et-hessienne]], [[critere-rt-s2]].
- Méthodes : [[etudier-points-critiques]], [[extremum-global]].

### 4.4 et 4.5 – Ordre $n$ et formules de Taylor
- [[classe-cn]] ; [[formules-de-taylor]] (Young, Lagrange, reste intégral).

## 🔑 Définitions / formules à retenir
| Terme | Formule |
|---|---|
| [[differentielle-seconde]] | $D^2f_a(h,k)=(D^2f_a(h))(k)$, bilinéaire symétrique |
| [[theoreme-de-schwarz]] | $\partial^2_{ij}f(a)=\partial^2_{ji}f(a)$ |
| [[matrice-hessienne]] | $H_f(a)=(\partial^2_{ij}f(a))$ ; en dim 2 : $\begin{pmatrix}r&s\\s&t\end{pmatrix}$ |
| [[taylor-young-ordre-2]] | $f(a+h)=f(a)+Df_a(h)+\frac12(rh_1^2+2sh_1h_2+th_2^2)+\lVert h\rVert^2\varepsilon(h)$ |
| [[point-critique]] | $Df_a=0$ |
| [[critere-rt-s2]] | $rt-s^2>0$ : extremum (min si $r>0$, max si $r<0$) ; $<0$ : selle ; $=0$ : pas de conclusion |
| $X\mapsto X^2$ | $D^2f_A(H,K)=HK+KH$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Écrire la formule de Taylor-Young à l'ordre 2 pour $g:\mathbb R^2\to\mathbb R$ au point $(a_1,a_2)$ (Écrit 2025-2026).
2. Énoncer le théorème de Schwarz.
3. Définir : extremum local, point critique. Montrer qu'un extremum local est un point critique.
4. Énoncer le critère $rt-s^2$. Que faire quand $rt-s^2=0$ ?
5. Points critiques et nature pour $f(x,y)=x^3-3x+y^2$, puis $f(x,y)=3xy-x^3-y^3$.
6. Dans quelle formule de Taylor faut-il que $f$ soit à valeurs réelles ?

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[cd-exercices-types-corriges]] (ex. 11, 12, 13) · pièges : [[cd-mes-erreurs]]
- Précédent : [[03-accroissements-finis]] · Suivant : [[05-inversion-locale-fonctions-implicites]]
- Source : [cours rédigé](fichiers/cd-cours-redige-ch1-5.pdf)
