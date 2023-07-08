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



### Développer le micro-service Immatriculation

<img width="958" alt="immatriculationService" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/df517b07-3880-474e-90a0-bba4ce56b85f">

   
<img width="356" alt="image" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/726a5a67-08fd-442b-aa4e-5bf53ee32ef7">

GRPC: All owner

<img width="701" alt="allowners-grpc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/cc1f5978-b071-4680-af1a-ea7c493ec1c9">
   
GRPC : edit owner

<img width="701" alt="editowners-grpc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/f32bacd6-888e-4110-9d15-3f022e5c93b5">

GRPC: one Owners
 
<img width="694" alt="oneowners-grpc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/a693c06e-c396-42c2-93d1-f096507dc741">

GRPC: all vehicules 

  <img width="687" alt="allVehicules-grppc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/42ad7290-5660-4288-9a03-e333d9e16298">

  GRPC: one vehicule 

  <img width="705" alt="onevehicules-grpc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/216c35c3-ff36-4dc0-a9c9-07270affc028">

GRPC: delete vehicule

<img width="712" alt="deletevehicule-grpc" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/37814693-fa09-4d5d-ba62-81f19fe176df">

REST : all owners 

<img width="652" alt="allowners-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/ebb7e1b2-65d1-4a19-99d1-3497c356ea3f">

REST : Edit owners 

<img width="638" alt="editowners-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/91f75520-ab7c-4bb5-8452-2378b1214016">

REST : one owner

<img width="665" alt="oneowner-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/5f139b80-2218-48c8-b479-1796671fa07d">


REST : All vehicules 

<img width="648" alt="allvehicules-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/40c7199e-f1f2-486f-9efc-1232277b36a9">

REST : one vihucles 

<img width="638" alt="onevehicules-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/b79d53a5-f79b-4d55-85da-b7aec992316b">


GRAPHQL: all vehicules

<img width="893" alt="allvehicules-graphQl" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/0ac1c26e-9d20-4ee3-8fb4-e5992711dd8c">

### Développer le micro-service Infraction

Rest: all infraction
   
<img width="647" alt="allinfraction-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/73fc77a3-1574-47c7-b0a0-84267d7a63aa">

Rest : one infraction

<img width="664" alt="oneinfraction-Rest" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/1776ba9e-ebb3-459d-9b15-ff8e3c007dd0">

### Développer le micro-service Radar
   
   <img width="938" alt="Radarservice" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/6ad6f2f6-e64a-40eb-895b-116715b1af27">

### Eureka discovery

<img width="936" alt="eurekadiscovery" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/ff32b2d1-dce6-4cd8-b30c-e588b59e64e0">

<img width="955" alt="image" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/12e9f809-e3cf-4ad7-8a99-cf2745c81934">

### Gateway

<img width="937" alt="gatewayService" src="https://github.com/HafidaaHatim/Infraction-Violation-Detection-System-in-radars/assets/130146750/36aa4280-b2e4-4657-abd0-2994607fcbea">

### Implémentation




      


   

   



         














 

   

