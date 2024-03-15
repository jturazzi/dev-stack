<h1 align="center">🐋 Dev Stack</h1>
<h3 align="center">Cette configuration offre un environnement de développement avec plusieurs services incluant un serveur web, une base de données, Adminer pour la gestion de base de données, un outil de surveillance de serveur de messagerie (Mailpit), Portainer pour la gestion des conteneurs Docker, et Traefik pour le proxy inverse.</h3>

## Utilisation

1. Clonez ce dépôt.
2. Accédez au répertoire.
3. Modifiez les variables d'environnement si nécessaire.
4. Lancez les conteneurs Docker : `docker-compose up -d`.

Accédez aux services :
- Serveur Web : [http://localhost](http://localhost)
- Adminer : [http://adminer.local](http://adminer.local)
- Mailpit : [http://mailpit.local](http://mailpit.local)
- Portainer : [http://portainer.local](http://portainer.local)

*Remarque : La configuration DNS est requise sur votre serveur DNS ou dans le fichier hosts pour atteindre les services.*

## Services

- Web : PHP-Nginx.
- Adminer : Gestion de base de données.
- DB : Serveur MySQL.
- Mailpit : Surveillance de serveur de messagerie.
- Portainer : Gestion Docker.
- Traefik : Proxy inverse.

## Configuration

1. Copiez le fichier `.env.example` et renommez-le en `.env`.
2. Ouvrez le fichier `.env` dans un éditeur de texte.
3. Modifiez les variables d'environnement selon vos besoins. Voici les variables disponibles :
   - `TZ` : Définissez le fuseau horaire (par défaut : Europe/Paris).
   - `MYSQL_ROOT_PASSWORD` : Définissez le mot de passe root de MySQL (par défaut : root).
   - `DEV_DOMAIN` : Définissez le domaine pour le développement local (par défaut : local).
4. Enregistrez le fichier `.env`.

## Licence

Ce projet est sous licence [MIT](LICENSE).
