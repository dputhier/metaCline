
Genomic
=======

Plan des tâches à effectuer pour la mise en place de la gestion des données génomiques (non clinique), auxquelles on y ajoutera les critères suivant:

**Structures des gènes** :

*Le client devra être capable de récuperer les différents paramètres suivants*

- Récupérer des exons
- Récupérer les SNP (single nucleotid polymorphism)
- Récupérer les mutations somatiques
- Récupérer les mutations les plus rares (types cancéreuses) à partir de la base donnée COSMIC (regroupe tous les types de mutants/variants)
- Identifier les sites de régulation
- Avoir le contenu Nt
- Table de passage
- Le pourcentage en %GC (ilôts CpG)
- Avoir la position du lieu des sites de régulation

Mettre en place la structure 3D du génome (chercher la structure sur PDB) /!\ surtout les paramètres structuraux /!\


Exploitation de la source de données externes (comparaison entre les données de l'utilisateur et des références)

Récuperer les bases de données en spécifiant ce qu'elles peuvent apporter (recherche lourde), prendre les assemblages des génomes des modèles (ainsi que d'autres espèces, validation avec le client des bases de données) ainsi que spécifier ce que les bases apportent vis-à-vis des caractéristiques et des paramètres étudiées.

On se focalisera principalement sur le phylum des eucaryotes (préférence du client).

  **Database:**
	
  Organismes modèles
	
* Génome Humain **GRCh37** & **GrCh38** (assemblage plus récent) [URL assemblage humain](https://www.ncbi.nlm.nih.gov/genome/guide/human/)
   + Critères apportés:
          -	Reference Genome Sequence
          -	RefSeq Transcript
          -	RefSeq Proteins
          -	dbSNP
          -	dbVar
          -	ClinVar
          -	RefSeq Reference Genome Annotation

* Assemblage *Mus Musculus* **GRCm38** [URL assemblage Mus Musculus](http://www.ensembl.org/Mus_musculus/Info/Index)
    + Critères apportés:
        -	Régulation
        -	Sequence Assemblage
        -	Variation (Variant/ phenotypes)
        -	Annotation Gene

* Assemblage *Zebrafish* **GRCz11** [URL assemblage Zebreafish/Danio rerio](http://www.ensembl.org/Danio_rerio/Info/Index)
    + Critères apportés:
        -	Régulation
        -	Annotation gène (plus de détail sur le lien)
        -	Variation
        -	Sequence assemblage

* Assemblage *C.Elegans* **WBcel235** [URL assemblage C elegans](http://www.ensembl.org/Caenorhabditis_elegans/Info/Index)
    + Critères apportés:
        -	Assemblage génomique
        -	Régulation
        -	Gène annotation (plus de détail sur le lien)
        -	Variation

* Assemblage *Drosophila Melanogaster*  [URL assemblage Drosophila Melanogaster](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview)
    + Critères apportés
        - Tous les détails sur le lien wiki de flybase

* Assemblage *Xenopus laevis* [URL assemblage Xenopus laevis](http://www.xenbase.org/entry/doNewsRead.do?id=136)

	
  ****

    Autres Espèces


