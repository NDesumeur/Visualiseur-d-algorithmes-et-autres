# Visualiseur d'Algorithmes

Plateforme web interactive pour visualiser et comparer des algorithmes de tri, graphes, structures de données et code assembleur. Zéro dépendances externes, pur JavaScript et CSS.

## Fonctionnalités

### Tri (Algorithmes de Tri)

Visualisez 14 algorithmes de tri avec animation en temps réel.

**Algorithmes disponibles:**
- Bulles, Insertion, Sélection
- Rapide (QuickSort), Fusion (MergeSort), Tas (HeapSort)
- Écart (ShellSort), Comptage (CountingSort), Cocktail, Radix
- Peigne (CombSort), Gnome, Cycle, Crêpe (PancakeSort)

**Contrôles:**
- Taille: ajuste le nombre d'éléments (5-120)
- Vitesse: change le délai entre les étapes (50-1200ms)
- Distribution: aléatoire, trié, inversé, presque trié
- Saisie manuelle: entrez vos propres nombres (3-120 éléments)
- Statistiques en direct: comparaisons et permutations comptabilisées

**Raccourcis clavier:**
- Espace: lecture/pause
- Flèche gauche/droite: navigation étape précédente/suivante
- R: regénérer tableau aléatoire

### Graphes

Explorez les algorithmes de recherche sur graphes: BFS, DFS et Dijkstra.

**Fonctionnalités:**
- BFS (Recherche en largeur): explore par niveaux
- DFS (Recherche en profondeur): explore par branches
- Dijkstra: calcule les plus courts chemins avec poids
- Sélecteur de nœud départ et cible (pour Dijkstra)
- Affichage des distances et reconstruction du chemin

**Contrôles:**
- Boutons radio: choisir l'algorithme
- Départ/Cible: sélectionner les nœuds
- Lecture/pause automatique des étapes
- Précédent/Suivant: navigation manuelle

**Graphe utilisé:**
6 nœuds (A-F) avec arêtes pondérées, prédéfini pour la démo.

### Structures de Données

Tab interactif pour expérimenter avec Pile et File.

**Pile (LIFO - Last In First Out):**
- Push: ajouter un élément au sommet
- Pop: retirer le sommet
- Affichage vertical, dernier en haut
- Historique des opérations

**File (FIFO - First In First Out):**
- Enqueue: ajouter à la fin
- Dequeue: retirer du début
- Affichage horizontal, défilement gauche-droite
- Historique des opérations

**Contrôles:**
- Saisie nombre
- Boutons Ajouter/Retirer/Vider
- Radio buttons pour basculer Pile/File

### Performances

Comparez les temps d'exécution de tous les algorithmes de tri.

**Données:**
- Taille: nombre d'éléments à trier (20-500)
- Runs: nombre de passages moyennés
- Tableau: Bouton "Comparer" pour benchmarker
- Résultats: table avec Algo, Temps (ms), Étapes
- Export: Copier les résultats en CSV pour feuille de calcul

### Assembleur

Simulateur x86-64 simplifié avec instructions et flags.

**Instructions supportées:**
- MOV: copier valeur en registre
- ADD/SUB: addition/soustraction
- CMP: comparer (définit flags ZF/SF)
- JMP: saut inconditionnel
- JE: saut si égal (si ZF=1)
- JNE: saut si non égal (si ZF=0)
- PUSH/POP: pile
- HALT: arrêt du programme

**Registres:**
RAX, RBX, RCX, RDX, RSI, RDI, RSP (pointeur pile), RBP (base pile)

**Exemples prêts à l'emploi:**
1. Boucle + somme: boucle comptant de 5 à 0, accumule dans RBX
2. Pile push/pop: empile deux valeurs, dépile et additionne
3. Branchement JE/JMP: compare avec CMP, saut conditionnel

**Contrôles:**
- Textarea: écrire ou éditer le code
- Sélecteur exemples: charger un programme
- Bouton Exécuter: lancer la simulation
- Précédent/Suivant: navigation pas à pas
- Lecture automatique: avancer tous les N ms
- Registres/Flags/Pile: affichés à chaque étape
- Code: surlignage de l'instruction courante

**Notes syntaxe:**
- Labels se terminent par ':' (ex: LOOP:)
- Les sauts utilisent le nom du label sans ':'
- Séparation d'arguments par virgules obligatoire
- Valeurs numériques ou noms de registre

### Raccourcis Clavier

Disponibles sur tous les onglets (sauf dans les champs de saisie):

- Espace: lecture/pause de l'animation
- Flèche gauche: étape précédente
- Flèche droite: étape suivante
- R: regénérer tableau (Tri seulement)

## Interface Utilisaire

**Thème:**
Fond bleu-gris foncé avec accents cyan/bleu ciel. Barres de progression dégradées pour une lisibilité optimale.

**Tabs:**
5 onglets pour naviguer: Tri, Graphes, Structures, Performances, Assembleur.

**Réactivité:**
Entièrement responsive sur mobile. Contrôles compacts, visualiseurs évolutifs.

## Installation et Usage

1. Ouvrir index.html dans un navigateur moderne (Chrome, Firefox, Safari, Edge)
2. Aucune installation, aucun serveur requis
3. Tous les calculs en local, zéro dépendances externes

## Notes Techniques

- Langage: JavaScript vanilla (ES6+)
- Style: CSS3 avec gradients et animations
- État: gestion centralisée via objet state
- Rendu: fonction render() mise à jour à chaque changement
- Performance: optimisée pour listes jusqu'à 120-150 éléments

## Cas d'Usage

- Enseignement: visualiser comment les algos fonctionnent étape par étape
- Apprentissage: comparer les performances réelles entre algos
- Débogage: tracer l'exécution de code assembleur
- Expérimentation: tester avec vos propres données
- Présentation: animer une explication d'algorithme en classe

## Améliorations Futures Envisageables

- Ajouter plus de structures de données (arbre binaire, hash table)
- Implémenter des algorithmes de graphe supplémentaires (Bellman-Ford, A*)
- Support pour DAG (graphes orientés acycliques) personnalisés
- Mode édition du graphe (ajouter/supprimer nœuds et arêtes)
- Enregistrement et partage de configurations
- Export SVG/PNG des visualisations

## Auteur
Par NDesumeur
Créé pour l'apprentissage interactif des algorithmes et structures de données.
