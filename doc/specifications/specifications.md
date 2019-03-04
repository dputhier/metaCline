#	Security functionality

## Utilisateurs

- Chaque utilisateur possède un login et un password
	- Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule, qui est crypté dans la bdd
	- Un login est unique, et un email est attribué à un login
	- Un mail est obligatoire pour s'inscrire
	- Un mail de confirmation est envoyé pour confirmer la possession du mail
	- Si un utilisateur perd son login ou mot de pass, il peut le recuperer en faisant une requête automatique auprès de l'administration \\\Lien équipe interface\\\
	- Chaque Login/password sera validé et renverra 'Logged' à l'interface ou 'Login/Password incorrect'. Au bout de 5 'Login/Password incorect' d'affilé, 'User locked' est envoyé  \\\Lien équipe interface\\\
		- Le compte est débloqué au bout de 12h (voir attribution chef de groupe)
		- À partir de 24h après la dernière tentative de mot de passe incorrecte, le compteur incorect est reinitialisé lors d'une nouvelle tentative de connection



## Gerer les groupes

- Chaque utilisateur peut demander à devenir un chef de projet et créer un groupe
  Chef de projet:
      - Un chef de projet peut choisir un utilisateur pour lui succeder
      - Un chef de projet gère son nom groupe 
      - UN chef de projet gère les personnes du groupe en autorisant leur entré, iil peut egalement les expulser du groupe et changer leur statut (voir statut groupe)
      - Un chef de groupe peut autoriser le déblocage d'un utilisateur présent dans son groupe avant les 12h.
      
##- Chaque utilisateur peut acceder à un groupe si le chef de projet le lui autorise, à differents niveaux (annotateur, statististicien, ...)
  statut groupe:
	  - Chef de projet (Tous les droits voir chef de projet definition) un seul par groupe 
	  - Sous chef (Tous les droits sauf l'ajout et suppression d'utilisateurs)
  	- 
  	-
	

		- 
		
## Administrateurs / ce sont les super user

- Les administrateurs ont accès à tous les groupes, ils ne sont pas membres officiel (dans la liste), mais ont tous les droits sur le groupe et les données qu'il contient
  - Les administrateurs peuvent occulter des fichiers
  - Les administrateurs ont accès aux fichiers
  - Les administrateurs autorisent ou pas un utilisateur à créer un groupe et devenir chef de projet

  - Les administrateurs n'ont pas accès aux mots de pass cryptés, mais peuvent débloquer un compte si un utilisateur le demande. 


Ordonné nos mots clefs exemple groupe doit apparaitre une fois que l'utilisateur, le chef, l'admin.

cryptage de base donnée ( entièrement bdd ) même les admins n'ont pas le droit , flux crypté

sauvegarde de données   (DUMP) rendre le serveur inhopérent pour pouvoir le faire 
si piraté changement de mot de passe avec mail de réinitialisation.

