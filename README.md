Bienvenue sur le projet lemonNode.js 
Ce projet est une nouvelle révolution dans l'univers du SSO.
Jusqu'à présent le SSO était une infrastructure complexe et fragile.
 
Avec lemonNode.js chaque application est capable d'embarquer son SSO. 

En effet lemonNode.js est très léger, il tourne sur tous les systèmes (unices et windows).
Par sa conception originale basée sur de la programmation asynchrone et des evenements non bloquants, il est capable de protéger une application tournant sur le même serveur.

Le moteur de lemonNode.js est le serveur javascript node.js

# Comment démarrer

## Prérequis:

node.js

npm

coffeescript (uniquement pour modifier les sources coffeescript)

## Dépendances

installer les modules : api_request ,node-uuid

npm install -g api_request

npm install -g node-uuid

## Lancement de lemonNode.js
### Le serveur de session et le fournisseur d'identité

LemonNode est livré avec un serveur de session en javascript et une application d'identification 

La commande 
  1001PX:~/lemonNode$ ./startservice.sh

Lance les deux  services 
 
  1001PX:~/lemonNode$ le serveur ecoute sur le port 8090

### lancement du reverse proxy 
  
  1001PX:~/lemonNode$ node lemonnode.js 

   Lancement de lemon:nodeJS
   le serveur lemon:nodeJS V0.0 ecoute sur le port 8080 
 
### modification du fichier /etc/hosts
 
Ajouter les deux lignes suivantes: 

   127.0.0.1       idp.demo.appli
   127.0.0.1       monintranet.demo.appli

### Test
   faire pointer son navigateur sur monintranet.demo.appli:8080


