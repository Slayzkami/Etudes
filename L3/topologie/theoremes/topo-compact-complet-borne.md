---
aliases:
  - "Un compact est complet et borné ; une partie compacte est fermée et bornée"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Un compact est complet et borné ; une partie compacte est fermée et bornée

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Prop. 3.18, 3.19 et Rem. 3.20 du cours (poly : Prop. 3.3, exercice 3.3, Rem. 3.1) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> 1. Si $(E,d)$ est compact, $E$ est **complet** et **borné**.
> 2. Une partie compacte $A$ d'un espace métrique est **fermée et bornée** dans $E$.
> 3. **Réciproques fausses** en général : $\mathbb R$ complet non compact ; $[0,1[$ borné non compact ; $\mathbb N$ discret fermé borné non compact.

> [!SUCCESS]- Démonstration
> *Borné* : $E=\bigcup_nB(a,n)$, on extrait un sous-recouvrement fini, donc $E=B(a,N)$.
> *Fermé (par les suites)* : soit $x_n\in A$, $x_n\to x\in E$. Par compacité, une sous-suite $x_{\varphi(n)}\to\ell\in A$ ; elle tend aussi vers $x$, donc $x=\ell\in A$ (unicité de la limite).
> *Borné (par les suites)* : sinon, pour $a\in A$ fixé, $x_n\in A$ avec $d(a,x_n)>n$ ; une sous-suite converge vers $\ell$, donc $d(a,x_{\varphi(n)})$ est bornée, alors que $d(a,x_{\varphi(n)})>\varphi(n)\ge n$.

## 🔗 Liens

- **S'appuie sur** : [[topo-partie-compacte|Partie compacte]], [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]], [[topo-suite-de-cauchy-espace-complet|Suite de Cauchy, espace complet]], [[topo-unicite-limite|Unicité de la limite]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-borel-lebesgue|Borel–Lebesgue : compacts de R et de R^n]]
- **Méthodes** : [[topo-montrer-non-compact|Méthode : montrer qu'une partie n'est pas compacte]]
- **Voir aussi** : —
