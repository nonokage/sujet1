#GitLab - Jenkins - SonarQube

Placez-vous dans le même répertore que le fichier docker-compose.yml et démarrez les conteneurs (le -d lance en tâche de fond):
```docker-compose up -d```

Pour vérifiez que les conteneurs sont bien lancés:
```docker ps```

Connectez-vous à localhost:10080 pour accéder à l'interface de GitLab.
identifiant: root
mot de passe: test1234

Connectez-vous à localhost:18080 pour accéder à l'interface de Jenkins.
Le mot de passe demandé est inscrit dans le log du conteneur Jenkins:
```docker logs <id du conteneur jenkins>```

Connectez-vous à localhost:19000 pour accéder à l'interface de SonarQube.
identifiant: admin
mot de passe: admin

Pour arrêtez les conteneurs:
```docker-compose down```# sujet1
