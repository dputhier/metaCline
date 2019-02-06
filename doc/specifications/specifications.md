---
output:
  html_document: default
  pdf_document: default
---
##Genomic

Plan de tâche à effectuer pour la mise en place de la gestion des données génomiques (non clinique), auquel on y ajoutera les critères suivant:

**Structure de gène** :

*le client devra être capable de récuperer les différents paramètres suivants*

- Récupérer des exons
- Récupérer les SNP (single nucleotid polymorphism)
- Récupérer les Mutation somatique
- Récupérer les Mutation les plus rares (types cancéreuses) à partir de la base donnée COSMIC (regroupe tous les types de mutant/variant)
- Identifier les sites de régulations
- Avoir le contenue Nt
- Table de passage
- Le pourcentage en %GC (ilôt cpG)
- Avoir la la position du lieux des sites de régulations

Mettre en place la structure 3D du génome (chercher la structure sur PDB) /!\ surtout les paramètres structuraux /!\


Exploitation de la source de donnée externe (comparaison entre les données de l'utilisateur et des références (Type de format de préférence ?))

Récuperer les bases de données en spécifiant ce qu'elle peut apporter (recherche lourde), prendre les assemblages des génomes des modèles (ainsi que d'autre espèce, validation avec le client des bases de données) ainsi que spécifier ce que les bases apportent vis-à-vis des caractéristiques et des paramètres étudiées.

L'utilisation des branches seront centrées sur les eucaryotes (préférence du client).

  **Database:**
	
	Espèce modèle
	
* Génome Humain **GRCh37** & **GrCh38** (assemblage plus récent) (link  : https://www.ncbi.nlm.nih.gov/genome/guide/human/ ) 
    + Critère apporter:
          -	Reference Genome Sequence
          -	RefSeq Transcript
          -	RefSeq Proteins
          -	dbSNP
          -	dbVar
          -	ClinVar
          -	RefSeq Reference Genome Annotation

* Assemblage *Mus Musculus* **GRCm38** (link  : http://www.ensembl.org/Mus_musculus/Info/Index)
    + Critère apporter:
        -	Régulation
        -	Sequence Assemblage
        -	Variation (Variant/ phenotypes)
        -	Annotation Gene

* Assemblage *Zebrafish* **GRCz11** (link  : http://www.ensembl.org/Danio_rerio/Info/Index)
    + Critère apporter:
        -	Régulation
        -	Annotation gène (plus de détail sur le lien)
        -	Variation
        -	Sequence assemblage

* Assemblage *C.Elegans* **WBcel235** (link  : http://www.ensembl.org/Caenorhabditis_elegans/Info/Index)
    + Critère apporter:
        -	Assemblage génomique
        -	Régulation
        -	Gène annotation (plus de détail sur le lien)
        -	Variation

* Assemblage *Drosophila Melanogaster* (link  : https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview)
    + Critère apporter
        - Tous les détails sur le lien wiki de flybase
	
  ****

	Autre Espèce


