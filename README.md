# Infraction-Violation-Detection-System-in-radars

1. Établir une architecture technique du projet
2. Établir un diagramme de classe global du projet
3. Développer le micro-service Immatriculation :
      a. Entités JPA et Interface JpaRepository basées sur Spring data
      b. Les 4 web services REST, GraphQL, SOAP et GRPC
      c. Tester les 4 web services
4. Développer le micro-service Infractions
5. Développer le micro-service Radar. Chaque dépassement de vitesse, ce service
devrait consulter le service d’immatriculation pour récupérer les informations sur le
propriétaire du véhicule. Ensuite il fait appel au service Infraction pour générer une
nouvelle infraction. La communication entre les services peut se faire au choix entre
REST, SOAP, GRPC ou GraphQL.
6. Créer un application java qui permet de simuler un radar qui génère aléatoirement
des dépassements de vitesses et de les envoyer, via GRPC, au service Radar-Service
7. Mettre en place les services techniques de l’architecture micro-service (Gateway,
Eureka Discovery service)
8. Développer votre application Frontend avec Angular ou React
9. Sécuriser votre système avec un système de d’authentification OAuth2 comme
Keycloak
10. Écrire un script docker-compose.yml pour le déploiement de ce système distribué
dans des conteneurs docker.



3. Développer le micro-service Immatriculation
   <img width="356" alt="image" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/726a5a67-08fd-442b-aa4e-5bf53ee32ef7">

   

