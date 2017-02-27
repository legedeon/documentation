# Serveur
## Lancer un petit serveur web dans un dossier
```bash
$ python -m SimpleHTTPServer
```
Un serveur web interprete toujours par defaut un fichier index.html la ou il a ete lance

pour ne pas avoir les logs, on redirige les logs vers /dev/null 
```bash
$ python -m SimpleHTTPServer > /dev/null 2>&1
```

## Utiliser le serveur web
Pour se connecter, on tape dans l'url du browser http://localhost:8000/
