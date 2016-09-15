# YouCraw
Crawler pour récupérer les méta-données YouTube, on utilisons l'API de Youtube, et la sauvegarde des méta-données dans une base de donénes MongoDB.
# Code Sources
# Dans le dossier ExtractYoutube, vous trouvriez le code source en java, développé avec l'IDE NetBeans 8.1

# Les méta-données disponibles

1. _id : l’identifiant de la vidéo
2. title : le titre de la vidéo
3. channelid : l’identifiant du canal
4. channeltitle : le titre du canal
5. datepub : la date de publication de la vidéo
6. description : la description de la vidéo
7. tags : une liste des mots liés à la vidéo
8. kind : le type par exemple youtube#video
9. defaultaudiolang : la langue par défaut de la vidéo
10. viewcount : le nombre du vue de la vidéo
11. likecount : le nombre des utilisateurs qui ont aimés la vidéo
12. dislikecount : le nombre des utilisateurs qui n’ont pas aimés la vidéo
13. commentscount : le nombre des commentaires
14. comments : une liste des commentaires
	(a) author : l’auteur du commentaire
	(b) like : le nombre des utilisateurs qui ont aimés le commentaire
	(c) message : le contenu du commentaire
15. transcription : la transcription de la vidéo

## Prérequis
1. OS Linux
2. MongoDB    https://www.mongodb.com/download-center?filter=enterprise#enterprise
3. Youtube-DL https://rg3.github.io/youtube-dl/
4. JAVA 1.8 ou supérieur
5. Python 2.7 ou supérieur
# Utilisation

1. Copier le dossier RUN_YOUTUBE dans votre machine
2. Création d'un compte Google sur le site https://developers.google.com/youtube/v3/getting-started
3. Récupération de fichier JSON qui contient le "clientId", "clientSecret"
4. Exécuter le script python "generateRefreshTokens.py" ou "getCredential.py" pour récupérer "refreshToken" 
5. Modifier les paramètres dans le fichier "YouCraw.sh"

## Lancer le Crawler
    $ ./YouCraw.sh

# Author : Saber
# Mail   : saber.lisis@gmail.com

# Licence
OpenSource
