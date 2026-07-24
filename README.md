# Pendule Double — Modélisation Numérique

**Projet INSA Lyon** — Modules de Modélisation Numérique

Simulation et analyse d'un **pendule double** — un système dynamique non linéaire présentant un comportement chaotique. Ce projet explore la résolution numérique des équations du mouvement, la quantification du chaos via les exposants de Lyapunov, et la visualisation de la dynamique complexe.

## 📋 Contenu

| Fichier | Description |
|---|---|
| `double_pendulum.ipynb` | Notebook Jupyter principal — simulation complète, analyse et visualisations |
| `pendule double.png` | Schéma du système pendule double |
| `diagramme de bifurcation legendé.png` | Diagramme de bifurcation annoté |
| `Schéma expliquation calcul exposant Lyapunov.png` | Explication du calcul des exposants de Lyapunov |
| `Ecart relatif heatmap final.png` | Heatmap de l'écart relatif (comparaison méthodes) |
| `Lyapunov Heatmap m1 = 0.1 m2 = 0.4 l1 = l2 = 0.5 bonne échelle.png` | Heatmap des exposants de Lyapunov |
| `Temps de retournement heatmap bons axes.png` | Heatmap du temps de retournement |
| `fig_compa_ana_num_2D.png` | Comparaison solution analytique vs numérique |
| `Animation theta10 = 175 theta20 = 10.mp4` | Animation — trajectoire chaotique (175°, 10°) |
| `Animation theta10 = 110 theta20 = 90.mp4` | Animation — trajectoire chaotique (110°, 90°) |

## 🧪 Méthodologie

### Résolution des équations différentielles

Les équations du mouvement du pendule double sont dérivées via le **formalisme de Lagrange** et résolues numériquement avec :

- **`scipy.integrate.solve_ivp`** / `odeint` — intégration numérique des ODEs
- **`numpy`** — calculs matriciels et manipulation des données
- Régime non linéaire (équations complètes) vs régime linéarisé (petites oscillations)

### Analyse du chaos

- **Exposants de Lyapunov** — quantification de la sensibilité aux conditions initiales
- **Diagrammes de bifurcation** — transition ordre → chaos
- **Temps de retournement** — métrique de stabilité du système
- **Heatmaps paramétriques** — influence des masses, longueurs et conditions initiales

### Visualisations

- Animations MP4 des trajectoires dans l'espace des phases
- Heatmaps 2D des exposants de Lyapunov
- Comparaison analytique vs numérique
- Diagrammes de bifurcation

## 🚀 Utilisation

```bash
# Cloner le dépôt
git clone https://github.com/<username>/double-pendulum.git
cd double-pendulum

# Lancer le notebook
jupyter notebook double_pendulum.ipynb
```

### Dépendances

- Python 3.x
- numpy, scipy
- matplotlib
- sympy (dérivation équations)
- ipywidgets, IPython.display (animations)

## 📊 Résultats clés

1. **Comparaison linéaire vs non linéaire** — le modèle linéarisé diverge rapidement du modèle non linéaire pour de grands angles
2. **Exposants de Lyapunov** — mise en évidence des régions chaotiques en fonction des paramètres physiques (masses, longueurs, angles initiaux)
3. **Diagramme de bifurcation** — visualisation de la transition vers le chaos
4. **Temps de retournement** — corrélation avec les exposants de Lyapunov pour caractériser la stabilité

## 📚 Références

- Strogatz, S. H. — *Nonlinear Dynamics and Chaos*
- Goldstein, H. — *Classical Mechanics* (formalisme de Lagrange)
- INSA Lyon — Cours de Modélisation Numérique

## 👤 Auteur

Projet réalisé dans le cadre des modules de Modélisation Numérique à l'INSA Lyon.