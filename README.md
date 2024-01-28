# Sujet du cours « Structure des bases de données relationnelles »

Vous êtes responsable informatique d'une école et on vous a demandé de concevoir une nouvelle base de données pour gérer l'activité de celle-là.

On a choisi une base de données relationnelles  pour sa robustesse, le fait que le code soit ouvert, et également pour sa popularité qui fait que beaucoup des personnes sont déjà formées à son utilisation.

Votre travail suivra le processus suivant :

1. Identification des données

Dans un premier temps,vous devrez recenser les données dont vous avez besoin pour les divers traitements que l'on vous demandera. Dans notre cas, il ne s'agit pas dela gestion exhaustive de l'école. Nous nous intéresserons principalement à la partie pédagogique. La question à laquelle vous devez répondre est la suivante : 
> Quelles sont les données nécessaires à la gestion des parcours étudiants au sein de l'école ?

2. Identification des « entités »

Dans un deuxième temps (ou en parallèle), vous aurez à identifier des entités qui permettent de regrouper les données. Cette partie du travail consiste donc à associer correctement les données aux entités, dans la perspective du modélisation relationnelle. Cette dernière est assez proche des modélisation objet pour ceux qui ont déjà utilisé des langages de programmation dits « orientés objet ».

L'objectif de cette phase est d'obter un modèle simple « **Entité/Association** » qui suit les principes de séparation du modèle entre :
- d'une part des entités qui représentent les objets de l'application
- d'autre part des associations qui représentent comment ces objets interagissent

Généralement, les associations sont assez bien décrits par des énoncés simples, comme par exemple :
```
Dans une activité de commerce, un commerçant achète des produits à un fournisseur
```
On voit ici que si l'on considère deux entités (Produit et Fournisseur), il existe une association « être fourni par » qui marque le lien **sémantique** entre les deux :
```
Produit <est-fourni-par> Fournisseur
```
D'une manière générale, une telle association est appelé un **prédicat**. 

3. Création du schéma de la base de données

La troisième étape consiste maintenant à implémenter votre modèle.

Normalement, les entités que vous avez dégagées doivent être transposables en tables de la base de données relationnelle. Vous devez maintenant prendre des décisions techniques :

- Quelle sera la **clef primaire** de chaque table ?
- Quels seront les **types** de chaque colonne des tables ?
- Quels **types d'associations** lient les tables entre elles ?
- Comment implémenter ces associations ?
- Comment implémenter des entités hiérarchisées ?

4. Vérification du schéma

Une fois votre schéma défini, Vous vérifierez que celui-ci ne comporte pas d'erreurs au regard des **formes normales** du calcul relationnel.


5. Rendu :
- Une courte analyse du problème (entre 1/2 et 1 page)
- Un diagramme Entité/Association représentant la structure de l'information
- Un schéma de base de données (sous forme d'export, par exemple)
- Une analyse des formes normales du schéma que vous avez conçu 
