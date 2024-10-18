# Projet-calculette
Cahier des charges simplifié :
1) Implémenter dans un premier temps une calculatrice permettant d’effectuer les opérations arithmétiques de base (addition, soustraction, multiplication, division) sur des nombres décimaux.
Cette calculatrice doit fonctionner en « notation polonaise inverse » : les différents opérandes sont empilés sur une pile de données (opération « push »), puis les différents opérateurs appliqués. Par exemple, pour réaliser l’addition de deux nombres :
- un premier nombre est saisi puis mis sur la pile (touche push),
- un deuxième nombre est saisi puis mis sur la pile (touche push),
- l’opération d’addition est appliquée (touche +).
Cette logique de fonctionnement est très pratique car elle permet de gérer des expressions complexes (par exemple 3*(2+5*(4+7)) sans le recours à des « mémoires » ou aux parenthèses.
2) Une fois cette première calculatrice implémentée, une première extension pourra être de lui ajouter un traceur de fonctions. Une autre extension pourra être de lui ajouter une fonctionnalité de calcul formel sur des polynômes.

Spécifications simplifiées de la calculatrice :
L’implémentation de la calculatrice doit respecter le patron de conception MVC (« Modèle », « Vue », « Contrôleur »). Ce patron spécifie qu’une application est composée de trois types d’éléments :
- des modèles, qui gèrent la représentation des concepts du systèmes (données et opérations de manipulation de ces données),
- les vues, qui gèrent les interfaces graphiques permettant les interactions avec l’utilisateur,
- les contrôleurs, qui gèrent les collaborations entre les vues et les modèles. Ainsi, les contrôleurs avertissent les vues des changements de valeurs d’un modèle afin qu’elles mettent à jour leur affichage. Inversement, les contrôleurs demandent aux modèles des changements de valeur pour refléter les actions des utilisateur (par exemple la saisie d’une valeur).
L’intérêt de ce patron de conception est de découpler (rendre indépendants) les vues et les modèles et de renforcer ainsi la modularité de l’application. Il est alors possible de changer les vues (modifier une interface, ajouter une interface) sans changer les modèles et inversement. L’impact de tels changements est alors limité au « connecteur » (le contrôleur) qui assure le lien entre la vue et le modèle.
