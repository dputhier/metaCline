# Interface/Visualisation #

### Cahier des charges ###


# Connexion #

Lors de l'ouverture du site, l'utilisatuer doit pourvoir choisir de se connecter à son compte ou de s'incrire (creer un compte).

## connexion a un compte existant ##
L'utilisateur doit renseigner dans un premier champs : "email ou pseudo "
Deuxième champs : "mot de passe"
Ces deux informations sont envoyées à la sécurité 
Si accepté connexion et affichage de l'interface suivante (utilisateur)
Sinon affichage message d'erreur (cf paragraphe Erreurs) + retour a l'interface de connexion

L'utilisateur doit pouvoir redemander un mot de passe en precisant son adresse email. **bold** A confirmer avec sécurité **bold**

##creation de compte ##

Lors de son inscription, on demande à l'utilisateur (les champs non falcultatifs sont obligatoires):
- un nom : "nom"
- un prenom: "prenom"
- un pseudo qui doit etre unique (facultatif)
- un adresse email (institutionnelle) "seul seront acceptée les email institutionnel les adresses gmail, hotmail ect ne seront pas acceptées"
- un mot de passe: "le mot de passe doit contenir " **bold** A confirmer avec sécurité **bold**
- une confirmation de mot de passe : "mot de passe"
- un organisme ou une institution de recherche: "nom de l'organisme/ institution d'affiliation"
- le pays de l'organisme ou de l'institution de recherche: selection d'un pays parmi la liste autorisée (menu déroulant)

affichage d'une interface " Demande de creation de compte en attente de validation "
	Chaque nouvelle inscription doit être validee ou refuser par les administrateur de MetaCline.
	**bold** Prevenir les utilisateurs que leur demande a été ou non validée par mail  SECURITE ? **bold**
retour a l'interface de connexion 

# Zone de l'utilisateur #

Chaque utilisateur doit pouvoir acceder ‡ sa zone propre.
Chaque utilisateur peut creer un groupe de travail.
Chaque utilisateur doit pouvoir acceder aux groupes de travail auxquels il a ete invite.
Chaque utilisateur doit pouvoir importer, exporter, modifier et supprimer des documents dans sa zone personelle.
Chaque utilisateur doit pouvoir importer, exporter, et modifer des documents dans sa zone de groupe.
Chaque utilisateur doit pouvoir acceder ‡ son historique (historique de recherche, historique des documents importes, historique des documents exportes).

# L'administrateur #

L'administrateur est un utilisateur qui dispose des droits du groupe de travail qu'il a cree.
(Il ne peut y avoir qu'un administrateur par groupe de travail.)
L'administrateur doit pouvoir designer un successeur qui disposera de tous les droits de l'administrateur. L'ancien administrateur devenant ainsi simple utilisateur.
L'administrateur doit pouvoir ejecter un utilisateur de son groupe de travail.

# L'interface #

L'utilisateur doit pouvoir choisir de se deconnecter.
L'utilisateur doit pouvoir voir prenom et nom lors de sa connexion, ou son pseudo si specifie.
L'utilisateur doit pouvoir acceder ‡ son profil lors qu'il clique sur son nom.

# Le profil #

Lorsque qu'un l'utilisateur exporter, importe, ou modifie un documents sur une zone de travail de groupe, les autres utilisateurs doivent pouvoir voir son nom et son prenom, et sa photo si disponible.
Sur l'espace profil, l'utilisateur doit pouvoir changer sa photo de profil, son mot de passe et son pseudo.
L'utilisateur peut choisir de supprimer son compte. Le compte sera supprime apres validation du choix de l'utilisateur.

# Gestion des donnees #

L'utilisateur doit disposer d'une fenÍtre pour effectuer des recherches sur la base de donnÈe et importer / exporter des documents.
Le site doit supoprter les documents en fichier txt, fasta, gtf et gff. **bold**Detailler plus tard chaque documents**bold**
