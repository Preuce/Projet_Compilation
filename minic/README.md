# DM de Compilation
LDD3 Magistère d'Informatique - Brice POINTAL et Alice PETIOT
## Tables des matières
0. [Enoncé](#ennoncé)
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Lignes de commandes](#lignesdecommandes)
4. [Extensions](#extensions)
***
## Enoncé
[Langages, interprétation, compilation
DM - Mini-C](https://www.lri.fr/~blsk/CompilationLDD3/dm-mnc.html)
***
## Introduction
L'objectif de ce DM est de construire la partie avant d'un compilateur pour un petit langage impératif correspondant à un fragment du langage C.
***
## Installation
Liste des technologies utilisées pendant ce projet:
* [Ocaml](https://ocaml.org/index.fr.html): Version 4.08.1
* [Menhir](https://opam.ocaml.org/packages/menhir/): Version 20200123
* [Dune](https://dune.build/): Version 2.1.3
***
## Lignes de commandes
* [compiler] : make minic.exe
* [compiler et tester] : make tests 
***
## Extensions

* [Etendre le langage] :
** Symboles : > , >= , <= , ==, || , &&, - (négation et soustraction), +, *
** Types : bool et void
** Autres fonctionnalités :
*** Boucle while, branchement if/if...else, instruction putchar(x)
*** Déclaration de variables (initialisées ou non)
*** Affectation de valeur aux variables
*** Déclaration de fonctions
*** Déclaration de variables locales
*** Appel de fonction n'utilisant pas de paramètre

* [Evaluer] : évaluation des expressions et des instructions

## Difficultés rencontrées
*Gestion des fonctions (déclaration et appel), particulièrement l'appel des fonctions usants de leurs paramètres dans leur code (déclenche l'erreur Not_found)
*Gestion de l'environnement (notamment local)