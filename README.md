#GitLab - Jenkins - SonarQube

Placez-vous dans le même répertore que le fichier docker-compose.yml et démarrez les conteneurs (le -d lance en tâche de fond):
<br>```docker-compose up -d```</br>

Pour vérifiez que les conteneurs sont bien lancés:
<br>```docker ps```</br>

Connectez-vous à localhost:10080 pour accéder à l'interface de GitLab.
Créez un nouveau mot de passe pour l'utilisateur root puis connectez-vous:
<br>identifiant: root</br>
<br>mot de passe: test1234</br>

Connectez-vous à localhost:18080 pour accéder à l'interface de Jenkins.
Le mot de passe demandé est inscrit dans le log du conteneur Jenkins:
<br>```docker logs <id du conteneur jenkins>```</br>

Connectez-vous à localhost:19000 pour accéder à l'interface de SonarQube.
<br>identifiant: admin</br>
<br>mot de passe: admin</br>

Pour arrêtez les conteneurs:
<br>```docker-compose down```</br>