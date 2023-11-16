# Docker-connection-DB

Sujet 1: Déployez une application multi-conteneurs en utilisant Docker Compose. L'application doit comprendre trois services : une application web (par exemple, WordPress), une base de données (par exemple, PostgreSQL) et un proxy inverse (par exemple, Nginx).

Tâches :

  Création du Fichier Docker Compose :

        Définissez un fichier docker-compose.yml pour les trois services.
        Configurez les variables d'environnement, les ports et les dépendances.

Dockerfile Personnalisé :
        Créez un Dockerfile pour le service de l'application web, en le personnalisant avec au moins une exigence spécifique (par exemple, installation de paquets supplémentaires, configuration de variables d'environnement).

    Persistance des Données :
        Configurez un stockage persistant pour le service de base de données à l'aide de volumes.

    Réseautage :
        Mettez en place un réseau personnalisé dans Docker et assurez une communication appropriée entre les conteneurs.

    Configuration du serveur Nginx   :
        Configurez du serveur Nginx comme proxy inverse pour diriger le trafic vers l'application web.



        Sujet 2 : Application PhpMyAdmin avec MySQL:

        Créez et déployez un fichier docker-compose pour créer deux services db et phpmyadmin en respectant la version 3

• db :  

             o Basé sur l’image : mysql:5.7
             o Publier le port 3306 du conteneur avec le port 6033 du l’hote  
             o Mappant un volume nommé bddata pour partager le code de l’application  
             o Requiert les variables d’environnements suivantes :  
                            o MYSQL_ROOT_PASSWORD o MYSQL_DATABASE  
                            o MYSQL_USER o MYSQL_PASSWORD  

• phpmyadmin:  

o Basé sur l’image phpmyadmin/phpmyadmin  

o Dépond du service db  

o Publier le port 80 du conteneur avec le port 8081 de l’hôte

              o Requiert les variables d’environnements suivantes :  
                     o PMA_HOST 
                     o PMA_PORT 

Sujet 3: Déployez une application complexe en utilisant Docker et Docker Compose. L'application doit inclure un service de traitement de données en temps réel (par exemple, Apache Kafka), une base de données NoSQL (par exemple, MongoDB), et une interface utilisateur web interactive (par exemple, une application React).

Tâches :

Création du Fichier Docker Compose :
        Définissez un fichier docker-compose.yml pour les trois services.
        Configurez les variables d'environnement, les ports et les dépendances.

    Dockerfile Personnalisé :

        Créez un Dockerfile pour le service de l'interface utilisateur, en le personnalisant avec au moins une exigence spécifique (par exemple, intégration d'un outil de monitoring).

    Persistance des Données :
        Configurez un stockage persistant pour le service de base de données en utilisant des volumes.

    Réseaux :
        Mettez en place un réseau Docker personnalisé et assurez une communication adéquate entre les conteneurs.
