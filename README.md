# Travaux sur les problématiques d'adressage

Afin d'améliorer le succès de géocodage des adresses, il nous a été nécessaire de 'normaliser' celles-ci.

Le travail a été réalisé en se basant sur des règles définies par les acteurs de l'adresse en terme d'abréviation et de façon empirique en travaillant sur les données en échec de géocodage.

## Normalisation

### Les types de voie

Le fichier ***type_voie_normalise.csv*** reprend les abréviations normalisées et leur type de voie.

Le fichier ***type_voie_normalise_perso.csv*** a été créé au fur et à mesure de découvertes d'abréviations non normalisées dans des fichiers des opérateurs.

### Les noms de voie

Le fichier ***nom_voie.csv***

Le fichier ***nom_voie_accent.csv*** rajoute les accents sur certains mots.

Exemples :
```csv
general,général
liberte,liberté
```

Le fichier ***nom_voie_article.csv*** rajoute des articles dans les noms.

Exemples :
```csv
mairie,de la mairie
république,de la république
```

**Nota : **Ce fichier est prévu pour traiter les cas où, le type de voie précède directement l'intitulé. Exemple : "Rue mairie"

Le fichier ***nom_voie_specifique.csv*** a été conçu spécifiquement pour corriger des valeurs saisies manuellement dans des bases opérateurs et ne respectant que peu de règles, étant tellement abrégées que toute tentative de géocodage est vouée à l'échec.

Exemples :
```csv
j j,jean-jacques
j f kennedy,kennedy
f et i,Frédéric et Irène
p et m,pierre et marie
```
