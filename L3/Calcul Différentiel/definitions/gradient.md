---
aliases:
  - "Gradient"
  - "∇f"
  - "grad f"
  - "gradient de f"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Gradient

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.39 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $f:\Omega\subset\mathbb R^n\to\mathbb R$ différentiable en $a$. Le **gradient** de $f$ en $a$ est le vecteur colonne
> $$\nabla f(a)={}^t\!\big(J_f(a)\big)=\begin{pmatrix}\frac{\partial f}{\partial x_1}(a)\\ \vdots\\ \frac{\partial f}{\partial x_n}(a)\end{pmatrix},\qquad Df_a(h)=\sum_{j=1}^n h_j\frac{\partial f}{\partial x_j}(a).$$

> [!TIP] À retenir
> - Le gradient n'existe que pour une fonction à valeurs **réelles**.
> - $a$ est un [[point-critique]] $\iff$ $\nabla f(a)=0$.
> - Plan tangent à $z=f(x,y)$ en $(a,b,f(a,b))$ : $z=f(a,b)+\partial_xf(a,b)(x-a)+\partial_yf(a,b)(y-b)$.

## 🔗 Liens

- **S'appuie sur** : [[matrice-jacobienne|Matrice jacobienne]]
- **Utilisé par (définitions)** : [[point-critique|Point critique]]
- **Méthodes** : [[calculer-jacobienne|Calculer une jacobienne et une différentielle sur R^n]], [[ecrire-taylor-young|Écrire la formule de Taylor-Young à l'ordre 2 en un point]]
