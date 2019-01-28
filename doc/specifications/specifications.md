#	Security functionality

## Gerer les groupes

- Chaque utilisateur peut demander à devenir un chef de projet et créer un groupe
- Chaque utilisateur peut acceder à un groupe si le chef de projet le lui autorise, à differents niveaux (annotateur, statististicien, ...):
	- Chef de projet (Tous les droits)
	- Sous chef (Tous les droits sauf l'ajout et suppression d'utilisateurs)
	- 
	-
	
- Un chef de projet peut choisir un utilisateur pour lui succeder
- Le chef de projet gère son nom groupe et les personnes du groupe

## Administrateurs

- Les administrateurs ont accès à tout les groupes
- Les administrateurs peuvent occulter des fichiers
- Les administrateurs autorisent ou pas un utilisateur à créer un groupe et devenir chef de projet

## Utilisateurs

- Chaque utilisateur possède un login et un password
	- Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule
	- Un login est unique, et un email est attribué à un login
- Un mail de confirmation est envoyé pour confirmer la possession du mail
