# learnrdemos
Démos pour introduire les concepts de [learnr](https://github.com/rstudio/learnr) and [gradethis](https://github.com/rstudio-education/gradethis), librairies RStudio de développement de tutoriels.

## Contenu

2 tutoriels sont proposés, chacun avec un fichier .rmd central, et des fichiers d'inclusion CSS et JavaScript : custom.css et header.html.

### Je code en R !

Ce tutoriel présente :

* 2 exercices de codage
* 1 QCU (questionnaire à choix unique) 
* un exemple de FlashCards
* un problème de Parsons

Les exercices de codage mettent en valeur le système des indices, progressivement révélés, et les mécanismes de vérification apportés par la librairie `gradethis`.

### Je fais un graphique !

Ce tutoriel présente :

* une illustration de la notion de *setup* et d'indépendance des environnements d'exercice
* 2 exercices de codage d'un graphique ggplot2

Différentes façons, équivalentes, de construire le graphique sont présentées. Le code de vérification est affiné pour pouvoir valider positivement des rédactions différentes, mais finalement justes.

## Installation

Le package peut s'installer de la façon suivante (ce qui a le mérite de mettre en place l'environnement permettant de développer d'autres tutoriels) :
```r
devtools::install_github("icem7-open/learnrdemos")
```
Les 2 tutos sont ensuite accessibles via l'onglet Tutorial de l'interface RStudio (en haut à droite).

## Compléments

### custom.css
Ce fichier de styles a deux fonctions :

* ajuster l'apparence graphique d'un tutoriel learnr : couleurs, polices, marges...
* déterminer le rendu alternatif, simplifié, si le tutoriel est diffusé dans une iframe


### header.html
Ce fichier comprend des blocs JavaScript pour mieux contrôler le rendu dynamique dans une iframe (ajustement dynamique de la hauteur d'un bloc d'exercice, selon qu'un indice est affiché ou que l'exercice déroule résultats et messages de correction), et la traduction de certains libellés.

