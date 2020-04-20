


https://www.hotelgedeon.com/product/
(il faudra renommer product en venteaemporter)
https://github.com/legedeon/hotelgedeon.com/tree/master/_product
https://github.com/legedeon/hotelgedeon.com/edit/master/_product/salade-caesar.md

chaque partie de la page venteaemporter est dans : https://github.com/legedeon/hotelgedeon.com/tree/master/_includes
la page principale : https://github.com/legedeon/hotelgedeon.com/blob/master/_layouts/default.html 
Les photos sont là : https://github.com/legedeon/hotelgedeon.com/tree/master/_product/mini-tof
Et devraient toujours être publiées avec une taille de 292x292 px (modifié) 

imagemagick : pour modifier la taille de toutes les images d'un repertoire
$ mogrify -resize 292x292^  -gravity center -crop 292x292+0+0 +repage *.jpg

jekyll est le moteur qui cree le fichier index.html en statique
jekyll est intégré à github
Pour installer jekyll : $ gem install bundler jekyll

Puis après pour lancer les serveur :
$ bundle exec jekyll serve

https://jekyllrb.com/docs/
