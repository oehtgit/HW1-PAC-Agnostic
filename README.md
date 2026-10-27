# Apprentissage statistique : PAC, convergence uniforme et No-Free-Lunch

Deux devoirs du cours *Statistical and Machine Learning*. Chacun vérifie par simulation (Monte-Carlo, NumPy) des résultats théoriques de l'apprentissage statistique.

## HW1 : PAC et PAC agnostique

[`HW1_PAC_Agnostic_CRETEL.ipynb`](HW1_PAC_Agnostic_CRETEL.ipynb)

- Classifieurs à seuil sur `[0, 1]`, appris par minimisation du risque empirique (ERM).
- **Cadre réalisable (PAC)** : sans bruit, la probabilité que l'erreur dépasse ε = 0,1 passe de 0,33 (m = 5) à 0 dès m = 50.
- **Cadre agnostique** : avec un bruit d'étiquette η = 0,1, l'erreur ne descend plus à 0. On mesure alors l'excès de risque par rapport au meilleur seuil.

## HW2 : Convergence uniforme et limites de l'apprentissage

[`HW2.ipynb`](HW2.ipynb)

- **Convergence uniforme** : variance du risque empirique en 1/√m, comparaison avec les bornes de Hoeffding et de l'union, effet de la taille |H| de la classe d'hypothèses, complexité d'échantillon expérimentale comparée à la valeur théorique.
- **No-Free-Lunch** : sur une cible aléatoire, aucun learner ne fait mieux que le hasard sur les points jamais vus.
- **Connaissance a priori** : si l'on sait que la cible est un seuil, l'ERM généralise même sur les points non vus. Avec m = 20 et N = 50, le risque est d'environ 0,04, contre 0,33 pour une cible aléatoire.

## Lancer

```bash
pip install numpy matplotlib jupyter
jupyter notebook
```
