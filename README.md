# Projet-BDD
Création d’une Base de Données à partir d’APIs
Dans ce projet, nous allons procéder à la création d’une Base de Données relationnelle via les plusieurs APIs.
Notre projet est intitulé « création et manipulation d’une Base de Donnée à partir d’API flight et API Covid ». Le choix de des APIs c’est dans le but de voir l’impact de la pandémie Covid-19 sur les flux aériens.
1.	Choix d’APIs :
Dans un premier temps, nous avons effectué le choix d’APIs, nous avons choisi plusieurs APIs de données Vols afin d’extraire des données complètes d’aéroport et des vols, et une API Covid qui porte des données sur tous les pays du monde ainsi que les données de nombre de cas positifs, nombre guéris, nombre de morts. Pour les APIs aériennes nous avons utilisés trois, (mot) API OpenSky qui nous permet de récupérer des informations sur l’espace aérien en direct. Dans notre projet   l’API utilisé d’OpenSky c’est API REST OpenSky qui récupère tous les vols d’un seul aéroport, c’est pour cette raison nous avons inclus une autre API qui est API Aerodatabox  qui contient une liste de tous les aéroport du monde. L’avantage de l’API REST OpenSky nous permets de récupérer des données à un intervalle de temps voulu et les dates voulues.
 API Aerodatabox contient des fonctionnalités utiles :  vols, statut des vols, retards de vol, horaires de vol, aéroports, horaires d'aéroport, indice de retard d'aéroport, statistiques de destination d'aéroport, heure locale d'aéroport, avions, images d'avion, reconnaissance d'image d'avion. Dans notre cas nous avons utilisé juste une liste des noms de tous les aéroports du monde dans REST API Open Sky. Nous n’avons pas utilisé d’autre données de cette API car nous offre uniquement des données qui datent récemment et un intervalle du temps des données des vols de huit heures. 
Dans notre Base de Données nous avons rajouté d’autres tables qui contient les informations détaillées pour chaque aéroport c’est pour cela nous avons rajouté la troisième API   airport-info.
API airport-info cette API comprend des informations détaillées sur un aéroport donné, telles que le nom complet, le site Web, les codes IATA et OACI, l’utilisation de cette API.
![image](https://user-images.githubusercontent.com/79981481/177039644-089aa6cd-4f25-4f8b-a573-5b9e5f13c62b.png)

2. Conception et administration de la base de données
 2.aCréation du modèle entité association
Dans un second temps, nous avons fait une identification des concepts et des entités qui composent le domaine fonctionnel, et les principaux attributs sur « le logiciel Diagrams.net » qui est un logiciel gratuit de diagrammes multiplateformes en ligne et de bureau. En effet, nous avons réalisé le Modèle Conceptuel des Données.
La figure suivante nous montre le Modèle conceptuel de la base de données.
 

2.b Création de la Base de Données sous SQL Server 
Après avoir modélisé le domaine fonctionnel de notre Base de Données avec UML, et effectué le Modèle Physique des Données, nous avons créé la base de données sous SQL server.

3.Remplissage de la Base de Données Covid Flight à partir d’APIs :
Après avoir conçu et administré la base de données, nous avons exécuté sous Jupyter NoteBook toutes les requêtes vers les APIs choisies, et le remplissage de la base de Données est effectué.

4. Extraction transformation et chargement de Données :
Après la récupération des Données des APIs et le chargement de ces données brutes dans notre Base de Données créée sous SQL Server, nous avons utilisé un autre outil qui est Power BI qui pour l’extraction et le nettoyage de ces données et création des relations entre les tables de notre base de données C’est une solution d'analyse de données de Microsoft et il nous permet de créer des visualisations de données personnalisées et interactives 
L’objectif dans cette partie consiste à analyser et visualiser l’impact de la covid sur l’espace airien.


