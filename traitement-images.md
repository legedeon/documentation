## DPI
Sur un ecran on a des images avec un resolution de 98 dpi
Une impression se fait a 266 dpi

Quand on a une image a 98 dpi si on veux voir a l'ecran comment elle va apparaitre en impression:
on sait que l'impression c'est environ 300 dpi, donc en gros 4 fois plus que 98 dpi
donc on fait un zoom de 400 %
Si on veux imprimer une image de 98 dpi correctement on va reduire sa taille de 4 avant impression

## Modifier la taille de l'image (pour qu'elle soit adaptee au site internet: par ex les 8 photos de la page d'accueil)
Sur GIMP Image / Echelle et taille de l'image
- 1 - Passer l'image en 98 dpi en changeant la resolution (pixel/inch) (car on veux une image pour l'ecran). ATTENTION c'est obligatoire car ca ne sers a rien de reduire une taille d'image sans reduire son contenu en dpi. On aurait une image reduite mais avec un poids inutilement important. 
- 2 - Changer la largeur ou la longueur, laisser du rab. Par ex: modif de 600 vers 400 en largeur va donner 320 au lieu des 300 souhaites.
- 3 - On ajuste la taille avec le canevas. Par ex: on ajuste le canevas pour passer de 320 a 300.
- 4 - Exporte l'image en jpg avec une qualite acceptable entre 60 et 80 
NB: penser a traiter les grandes images en premier. 
Par ex si on pars d'une image de 5000 par 3000, on cree la premiere image, la plus grande, de 600 par 400, puis on cree l'image vignette de 400 par 300. On ne fait JAMAIS l'inverse.



## Niveaux
Pour modifier les niveaux de tons dans une image: Couleurs / Niveaux
On voit le graphique du nombre de pixels par ton
On peut ajuster pour enlever les tons ou il n'y a pas beaucoup de pîxels

## Rognage, recadrage
Utiliser l'option : image > Taille du canevas

## Liens

### DPI
> https://fr.wikipedia.org/wiki/Point_par_pouce  
> http://blog.arnaudfrich.com/photo/pour-en-finir-avec-les-72-dpi/  
> http://sebsauvage.net/comprendre/dpi/  

### Niveaux
> [niveaux](http://www.ordissinaute.fr/ordissimo/fiche-pratique/2016-11-09-gimp-ameliorer-le-contraste-la-luminosite-et-les-couleurs-d-une-photo)

### Optimisation d'images
Avec jpegoptim:
find -type f -name "*.jpg" | xargs jpegoptim --strip-all
Avec optipng:
find -type f -name "*.png" | xargs optipng -il -nc -o7 -full
