# Interface/Visualisation #

### Cahier des charges ###


# Connexion #

Lors de l'ouverture du site, l'utilisateur doit pourvoir choisir de se connecter à son compte ou de s'incrire (creer un compte).
Suivant sur quel bouton il appuie, il est alors envoyé vers deux interfaces différentes

## connexion a un compte existant ##
L'utilisateur doit renseigner dans un premier champs : "email ou pseudo "

Deuxième champs : "mot de passe"

Ces deux informations sont envoyées à la sécurité 

Si acceptées: connexion et affichage de l'interface suivante (utilisateur)

Sinon: affichage message d'erreur (cf paragraphe Erreurs) + retour a l'interface de connexion

L'utilisateur doit pouvoir redemander un mot de passe en precisant son adresse email. **A confirmer avec sécurité**

##creation de compte ##

Lors de son inscription, on demande à l'utilisateur (les champs non facultatifs sont obligatoires): #quels sont les champs obligatoires/facultatifs? à preciser svp
- un nom : "nom"
- un prenom: "prenom"
- un pseudo qui doit etre unique (facultatif)
- un adresse email (institutionnelle) "seul seront acceptés les emails institutionnels, les adresses gmail, hotmail ect ne seront pas acceptées" #Merci de preciser pourquoi?
- un mot de passe: "le mot de passe doit contenir " **A confirmer avec sécurité**
#Selon sécurité: Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule
- une confirmation de mot de passe : "mot de passe"
- un organisme ou une institution de recherche: "nom de l'organisme/ institution d'affiliation"
- le pays de l'organisme ou de l'institution de recherche: selection d'un pays parmi la liste autorisée (menu déroulant)

affichage d'une interface " Demande de creation de compte en attente de validation"

	Chaque nouvelle inscription doit être validee ou refuser par les administrateur de MetaCline.
	**Prevenir les utilisateurs que leur demande a été ou non validée par mail  SECURITE ?**
	
Retour a l'interface de connexion.

# Interface utilisateur #

### zone profil ###

L'utilisateur doit pouvoir acceder à son profil complet lors qu'il clique sur son nom(/pseudo) situé en haut a droit de l'interface (cf profil)

Lorsque l'utilisateur clique sur le bouton fleche situé juste a coté de son nom(/pseudo) il a acces a un menu déroulant avec les raccourcis suivant:
- Administrateur (apparaît uniquement pour les utilisateur ayant un statut administrateur): renvoie sur l'interface administation
- Groupe: renvoie sur l'interface groupe 
- Déconnexion : permet de quitter la session renvoie sur l'interface de connexion

## zone recherche ## 
Lorsque l'utilisateur clique sur le bouton loupe/search situé en haut a gauche de l'interface, il a acces a la page de recherche 

## zone Historique ## 
Sous la Zone recherche est presente une zone historique sous forme d'une colone qui permet a l'utilisateur de voir immédiatement les 5 dernières recherches /modifications effectuée. 
Cela permet un acces rapide au resultat en cliquant sur la recherche/ modification d'intérêt. 
En bas de cette colonne ce trouve un bouton "voir plus" qui renvoie l'utilisateur sur l'interface historique #l'historique garde en mémoire toutes les recherches depuis la creation du compte? et il possible de le supprimer?

## zone groupe activity ##
La moitié de l'interface restante est dédiée a l'affichage des modification recentes apportées sur les différents groupes (10 au total tout groupe confondu) au quel l'utilisateur appartient. 
Cliquer sur les modifications renvoie directement l'utilisateur dans l'interface groupe et niveau de la dite modification. 
cliquer sur le titre de cette zone "groupe activity" renvoie l'utilisateur sur une interface qui affiche toute l'actualité des groupes

## zone document personnel ##
l'autre moitié restante est dédiée à l'affichage des documents stockés personnellement sur le serveur et l'import / export de documents.
En cliquant sur le titre "documents personnels" renvoie l'utilisateur renvoie sur une interface documents personnels #Attention phrase incompréhensible

affichage d'un champs Import : " déposer un sélectionner un fichier au format **A confirmer avec l'équipe en charge des analyse/ base de données** # à reformuler
permet de déposer glisser un fichier a importer dans la zone documents personnels ou de sélectionner le fichier sur la machine par un menu deroulant/ finder. # la zone se nomme document personnel ou documments personnels?

affichage d'un champs Export : " sélectionner un fichier à télécharger" 
 sélectionner un fichier  des documents personnel pour le télécharger localement. 


# interface documents personnels #
affiche la totalité des documents sauvegardés sur le serveur par l'utilisateur. 
En cliquant sur le document permet de le modifier (renommer ect),de l'ouvrir, de l'exporter ou le supprimer. #a reformuler
Lors de la suppression apparait un message : "etes vous sur de vouloir supprimer ce document: Oui  Non"
si l'utilisateur sélectionne oui suppression definitive du document puis retour a l'interface, si non retour a l'interface documents personnels. 

# Interface groupe activity #
a completer

# Interface Historique # 
a completer

# Interface recherches #
a completer

# Interface administrateur #

L'administrateur est un utilisateur qui dispose des droits du groupe de travail qu'il a cree.
(Il ne peut y avoir qu'un administrateur par groupe de travail.)
L'administrateur doit pouvoir designer un successeur qui disposera de tous les droits de l'administrateur. L'ancien administrateur devenant ainsi simple utilisateur.
L'administrateur doit pouvoir ejecter un utilisateur de son groupe de travail.


# Interface profil #

L'utilisateur doit pouvoir choisir de se deconnecter.
Lorsque qu'un l'utilisateur exporte, importe, ou modifie un document sur une zone de travail de groupe, les autres utilisateurs doivent pouvoir voir son nom et son prenom, et sa photo si disponible.
Sur l'espace profil, l'utilisateur doit pouvoir changer sa photo de profil, son mot de passe et son pseudo.
L'utilisateur peut choisir de supprimer son compte. Le compte sera supprime apres validation du choix de l'utilisateur.

# Interface Groupe #
 a completer 


# Gestion des donnees #

L'utilisateur doit disposer d'une fenêtre pour effectuer des recherches sur la base de donnée et importer / exporter des documents.
Le site doit supoprter les documents en fichier txt, fasta, gtf et gff. **Detailler plus tard chaque document**
