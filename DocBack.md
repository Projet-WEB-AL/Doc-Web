# Rendu Back

Ce document rend compte du travail effectué pour le TP web.


## Un tp guidé

etant donné que ce TP se base sur un tutoriel, nous avons eu tres peu de marge de maneuvre sur cette partie la.


## Technologies Utilisés

Nous avons utilisé un framework Node.js appelé Nest.js pour créer notre back.

Ce framework permet d'avoir une conformitée dans la facon de développer le backEnd de notre site. Il nous permet de construire notre site, module par module.

Le language utilisé est le TypeScript, un dérivé de java stript fortement typé. Il permet une meileur structure du code en permettant de definir des types.


## Percistance des donnés

Pour sauvegarder les données, ils nous fallait une base de donnée. Dans le sujet, la base de donnée conseilée est SQLight.

Nous avons choisis MySql, car nous l'avions déja utilisée au paravant.


## Relations 

Association : User 
Une relation many to many est la plus logique. Etant donné qu'une association peut contenir plusieurs users

Pour les roles, nous n'avons pas fini l'implémentation, mais il s'agirait du meme type de relation.


## Les modifications apportés au sujet.

- Désormais, le login prend un username en entrée, au lieux de prendre un ID, cela facilite la connection des utulisateurs.

    Pour répondre au besoin de cette modification, le backend à du recevoir quelques ajouts de methodes, comme ajouter un champ 'pseudonyme' au type User.

    Il a fallut évidement ajouter ces répercutions dans les methodes CRUD, et ajouter une façon d'etre sur que le pseudonyme soit unique.

- Afin de pouvoir trier les utilisateurs en fonction d'un attribut, nous avons du également créer une methode de tri dans le backend. Nous avons égélement fait le choix de mettre cette fonctionnalité dans le backend, car nous sommes sur de sa puissance comparé aux machines utilisateurs
