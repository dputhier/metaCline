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

## Administrateurs #l'equipe securite suggere un seul administrateur par groupe cela vous semble correct?

- Les administrateurs ont accès à tout les groupes
- Les administrateurs peuvent occulter des fichiers
- Les administrateurs ont accès aux fichiers
- Les administrateurs autorisent ou pas un utilisateur à créer un groupe et devenir chef de projet
- Chaque administrateur possède un login et un password
	- Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule
	- Un login est unique, et un email est attribué à un login
- Les administrateurs ont accès aux mots de pass cryptés

## Utilisateurs

- Chaque utilisateur possède un login et un password
	- Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule
	- Un login est unique, et un email est attribué à un login
	- Un mail est obligatoire pour s'inscrire
	- Si un utilisateur perd son login ou mot de pass, il peut le recuperer en faisant une requête automatique auprès de l'administration \\\Lien équipe interface\\\
	- Chaque Login/password sera validé et renverra 'Logged' à l'interface ou 'Login/Password incorect'. Au bout de 5 'Login/Password incorect' d'affilé, 'User locked' est envoyé  \\\Lien équipe interface\\\
		- Le compte est débloqué au bout de 12h
		- Un chef de groupe peut autoriser le déblocage d'un utilisateur présent dans son groupe avant les 12h.
		- À partir de 24h après la dernière tentative de mot de passe incorrecte, le compteur incorect est reinitialisé lors d'une nouvelle tentative de connection
		
- Un mail de confirmation est envoyé pour confirmer la possession du mail


Ordonné nos mots clefs exemple groupe doit apparaitre une fois que l'utilisateur, le chef, l'admin.

cryptage de base donnée ( entièrement bdd ) même les admins n'ont pas le droit , flux crypté

sauvegarde de données   (DUMP) rendre le serveur inhopérent pour pouvoir le faire 
si piraté changement de mot de passe avec mail de réinitialisation.

