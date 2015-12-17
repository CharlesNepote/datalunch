# Géocoder un fichier .csv d'adresse


- **Niveau** : Débutant / **Intermédiaire** / Avancé / Expert
- **Auteur** : VB
- **Date de MàJ** : 17/12/2015
- **Licence** : CC-by-sa

## Principes - Ce que nous allons faire
À partir d'un fichier contenant des adresses, encodé en .csv, nous allons "géocoder" (définir les longitudes et lattitudes) ces adresses pour permettre ensuite d'en faire, par exemple une carte.

## Ingrédients - Ce dont nous avons besoin
Un fichier .csv contenant des colonnes d'adresses
une connection internet

## Étapes - Comment allons-nous procéder ?
### Géocodage des données
* On va se servir de Addok, géocodeur : http://adresse.data.gouv.fr/csv/
* on y importe le fichier sonnom.csv,
* on glisse les colonnes adresse,
* ville qui nous intéresse pour le géocodage,
* on sélectionne le code postal correspondant,
* on s'assure d'avoir le bon encodage (pas de caractères anormaux dans la prévisualisation).
* On clique sur Lancer et on récupère un fichier en sonnom.geocoded.csv, qui comprend toutes les informations de sonnom.csv, plus des colonnes supplémentaires avec lattitude, longitude, l'adresse que cela renvoie, si c'est un numéro de rue, de maison, de ... code insee, et un result_score

### Vérification du géocodage
On ouvre le fichier sonnom.geocoded.csv et en particulier on regarde le result_score. On vérifie aussi le result_city, contexte, ...
Si il est trop proche de zéro, il y a des erreurs
Si il est proche de un, on est bon !


## Aller + loin : 
Quelques sources : 

## A savoir : 

## Liens avec d’autres fiches : 