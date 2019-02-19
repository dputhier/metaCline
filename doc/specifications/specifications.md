# Interface/Visualisation #

### Cahier des charges ###


# Connexion #

Lors de l'ouverture du site, l'utilisateur doit pouvoir choisir de se connecter à son compte ou de s'inscrire (créer un compte).
Suivant sur quel bouton il appuie, il est alors envoyé vers deux interfaces différentes.

## connexion a un compte existant ##
L'utilisateur doit renseigner dans un premier champs : "email ou pseudo "

Deuxième champs : "mot de passe"

Ces deux informations sont envoyées à la sécurité .

Si acceptées: connexion et affichage de l'interface suivante (utilisateur).

Sinon: affichage message d'erreur (cf paragraphe Erreurs) + retour a l'interface de connexion.

L'utilisateur doit pouvoir redemander un mot de passe en précisant son adresse email. **A confirmer avec sécurité** # sécurité precise: Si un utilisateur perd son login ou mot de passe, il peut le recupérer en faisant une requête automatique auprès de l'administration. 

## creation de compte ##

Lors de son inscription, on demande à l'utilisateur (les champs non facultatifs sont obligatoires):
- un nom : "nom"
- un prenom: "prenom"
- un pseudo qui doit être unique (facultatif)
- un adresse email (institutionnelle) "seul seront acceptés les emails institutionnels, les adresses gmail, hotmail ect ne seront pas acceptées"
- un mot de passe: "le mot de passe doit contenir " **A confirmer avec sécurité**
#Selon sécurité: Un password possède minimum 8 caractères dont 1 chiffre, une minuscule et une majuscule
- une confirmation de mot de passe : "mot de passe"
- un organisme ou une institution de recherche: "nom de l'organisme/ institution d'affiliation"
- le pays de l'organisme ou de l'institution de recherche: selection d'un pays parmi la liste autorisée (menu déroulant)

Affichage d'une interface " Demande de création de compte en attente de validation"

Chaque nouvelle inscription doit être validée ou refuser par les administrateurs de MetaCline.
**Prevenir l'utilisateur que sa demande a été ou non validée par mail  SECURITE ?**
	
Retour à l'interface de connexion.

# Interface utilisateur #

Une image pour vizualiser plus facilement la disposition des zones sera jointe ici.

### zone profil ###
L'utilisateur doit pouvoir accéder à son profil complet lorsqu'il clique sur son nom(/pseudo) (cf profil).

Lorsque l'utilisateur clique sur le bouton flèche, il a accés à un menu déroulant avec les raccourcis suivants:
- Administrateur (apparaît uniquement pour les utilisateur ayant un statut administrateur): renvoie sur l'interface administation
- Groupe: renvoie sur l'interface groupe 
- Déconnexion : permet de quitter la session renvoie sur l'interface de connexion

## zone recherche ## 
Lorsque l'utilisateur clique sur le bouton loupe/search, il a accés à la page de recherche.
Avec la barre de recherche, sont présents deux filtres: le premier permet de filtrer le type de données (exemple: ne chercher que parmi les exons, ou les SNP...), tandis que le deuxième permet de filter les génomes (exemple: ne chercher que parmi le génome humain hg38). Ces deux filtres peuvent être combinés, être utilisés seuls, ou laissés vides. Par défaut, ces filtres sont vides est la recherche est effectuée parmi tout les types de données et tout les génomes.

## zone Historique ## 
Est présente une zone historique sous forme d'une colonne qui permet à l'utilisateur de voir immédiatement les 5 dernières recherches/modifications effectuées. 
Cela permet un accés rapide aux resultats en cliquant sur la recherche/ modification d'intérêt. 
En bas de cette colonne ce trouve un bouton "voir plus" qui renvoie l'utilisateur sur l'interface historique.

## zone groupe activity ##
La moitié de l'interface restante est dédiée à l'affichage des modifications récentes apportées sur les différents groupes (10 au total tout groupe confondu) auquel l'utilisateur appartient. 
Cliquer sur les modifications renvoie directement l'utilisateur dans l'interface groupe et au niveau de la dite modification. 
Cliquer sur le titre de cette zone "groupe activity" renvoie l'utilisateur sur une interface qui affiche toute l'actualité des groupes.

## zone documents personnels ##
La moitié restante est dédiée à l'affichage des documents stockés personnellement sur le serveur et l'import / export de documents.
En cliquant sur le titre de la zone "documents personnels" renvoie l'utilisateur sur l'interface des documents personnels.

Affichage d'un champs Import : " déposer un sélectionner un fichier au format **A confirmer avec l'équipe en charge des analyse/ base de données** 
Permet de déposer glisser un fichier a importer dans la zone documents personnels ou de sélectionner le fichier sur la machine par un menu deroulant/finder. 

Affichage d'un champs Export : " sélectionner un fichier à télécharger" 
 sélectionner un fichier des documents personnels pour le télécharger localement.

# interface documents personnels #

Affiche la totalité des documents sauvegardés sur le serveur par l'utilisateur.

En cliquant sur le document cela permet de le modifier (renommer ect), de l'ouvrir, de l'exporter ou le supprimer.
Lors de la suppression apparait un message : "êtes-vous sur de vouloir supprimer ce document: Oui  Non"
Si "oui" est séléctionné par l'utilisateur, cela suprime définitivement le document puis retourne automatiquement l'utilisateur à l'interface des documents personnels. Si "non" est séléctionné, alors l'utilisateur est retourné à l'interface des documents personnels sans modification du document.. 

# Interface Historique # 

Affiche une liste classée de facon chronologique inverse de toutes les recherches (dans la limite de l'espace mémoire alouée à cette partie du site), import/export de fichier.
Cliquer sur une recherche permet d'accéder aux résultats de celle-ci.

Se trouve également un bouton "effacer l'historique" : fait apparaitre des cases à cocher devant les éléments de l'historique et affiche 2 boutons supplémentaires : "supprimer les éléments sélectionnés", et "tout sélectionner".
Aprés avoir sélectionner les cases à supprimer (ou avoir cliquer sur "tout sélectionner"), l'utilisateur doit cliquer sur "supprimer les éléments sélectionnés" pour finaliser la suppression. 

La zone profil continue d'apparâitre pour un accés rapide (cf interface utilisateur).

# Interface groupe activity #

Affiche un "historique" qui recense tous les changements effectués dans les différents groupes auquels appartient l'utilisateur.
Les résultats apparaissent classés de façon chronologique inverse. 
Chacun d'entres eux sont cliquables. 

La zone profil continue d'apparâitre pour un accés rapide (cf interface utilisateur).
 
# Interface recherches #
Permet de réaliser les tests statistiques définis par l'équipe stat
Ces résultats peuvent être exporter:
	- en pdf: hors du site et directement sur l'ordianteur personel de l'utilisateur
	- partagés avec d'autres utilisateurs du site: postés dans un groupe (cf interface groupe)

# Interface administrateur #

L'administrateur est un utilisateur qui dispose des droits du groupe de travail qu'il a créé. (Il ne peut y avoir qu'un administrateur par groupe de travail.)

L'administrateur doit pouvoir désigner un successeur qui disposera de tous les droits de l'administrateur. L'ancien administrateur devenant ainsi que simple utilisateur.
L'administrateur doit pouvoir éjecter un utilisateur de son groupe de travail.


# Interface profil #

Sur l'espace profil, l'utilisateur doit pouvoir changer sa photo de profil.
Il y a un champ qui permet de modifier son mot de passe. 
Demande une confirmation.

L'utilisateur peut cliquer sur "supprimer mon compte". Le compte sera supprimé apres validation du choix de l'utilisateur.
L'utilisateur peut cliquer sur "déconnection". Cela renvoie l'utilisteur sur l'interface de connexion.

# Interface Groupe #
Les utilisateurs appartenant au groupe peuvent poster les résultats de leur recherche.
Les autres utilisateurs ne peuvent pas modifier les résultats de la recherche.
Tous les utilisateurs appartenant au groupe peuvent commenter un post.
Les posts s'affichent dans le groupe en ordre chronologique inverse.
Seuls les posts s'affichent par défaut sur l'interface de groupe, et c'est seulement en cliquant dessus qu'un utilisateur appartenant au groupe peut voir les résultats postés et les commentaires.

# Gestion des données #
Le site doit supporter les documents en fichier txt, fasta, gtf et gff. **Détailler plus tard chaque document**
