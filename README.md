# Résumé du projet
Un siteweb utilisant 12 replicas qui lie à Nextcloud, une application qui donne accès à des fichiers personnels et qui permet de partager ces fichiers ainsi que de monitorer les échanges de fichiers grâce à une base de donnée (en l'occurence MariaDB ici) de façon sécuritaire. On intègre aussi Mattermost, un serveur de clavardage, étant utilisé comme alternative à Slack.



# Temps pour la réalisation du projet: environ ~6 heures

# Difficultés

Il n'y en a pas vraiment eu, sauf que j'ai perdu beaucoup trop de temps sur un problème stupide: la connection entre Nextcloud et MariaDB. Je n'avais pas réalisé que le selecteur du service pour MariaDB devait référencer le label du deploiement de MariaDB et non le metadata: name: de celui-ci, donc la connection de Nextcloud était refusé.
J'ai aussi eu quelques difficultés avec le lien entre github et docker hub. J'ai fais un push du projet sur Github avant de faire le lien, donc l'automatisation de Docker Hub ne faisait pas le build pour le projet qui était déjà sur released sur Github.

![Screenshot](https://github.com/Excelsis27/420-4d4-es/raw/main/2021-05-24.png)


### M-A-J par A.B.
