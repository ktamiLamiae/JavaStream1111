## Ktami Lamiae
## Nom de projet :  Application de Matching Compétences-Opportunités avec IA
## Description du diagramme UML
<img src="./UmlAI.png" width="600">
Ce diagramme représente une application simple de matching compétences ↔ opportunités, utilisant héritage et une interface.

## Interface

IAuthenticable : définit deux méthodes, login() et logout(), pour tous les utilisateurs du système.

## Classe abstraite

User : classe de base pour tous les utilisateurs, avec les attributs id et email.

## Héritage

Candidate hérite de User et possède un attribut name.
Chaque candidat est lié à un Profile contenant un résumé ou une biographie.
Recruiter hérite de User et possède un attribut companyName.
Chaque recruteur peut publier plusieurs Opportunity (offres d’emploi).

## Relations

Candidate → Profile : chaque candidat possède un profil.
Recruiter → Opportunity : chaque recruteur peut publier plusieurs opportunités.
