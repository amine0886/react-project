# react-project


Rapport du TP
donc ce tp on va le applique avec le react et nodejs Express et on va utilisé docker

on a fais des modification sur notre l’interface du notre projet
pour 

<img width="482" alt="Capture1" src="https://user-images.githubusercontent.com/98590213/169669815-4d901f60-f6a4-4703-a909-977178d09ff2.PNG">

pour registrer un nouveau utilisateur 
<img width="483" alt="Capture2" src="https://user-images.githubusercontent.com/98590213/169669820-1f0ef85c-e162-4c75-a0c7-053fc3cee2ba.PNG">
 et la on a ajouter aussi des message d'erreur d enregistrement ou d'user a ete enregistrer
 <img width="466" alt="Capture3" src="https://user-images.githubusercontent.com/98590213/169670017-f850a1ed-4759-494a-8d41-a78dcefac615.PNG">

 et utilisateur enregistrer 
<img width="468" alt="Capture4" src="https://user-images.githubusercontent.com/98590213/169670020-aa003f83-ac0e-45da-bd0e-c4bef10469f4.PNG">

*l objectif de TP et de applique le react front end pour publié l’interface sur le web via des centenaire et pour cela on va utilisé le docker
-commençons ai début par installation du docker sur notre machine Windows 
-activation de hyper-v et conteneur sur la machine pour pouvoir être accédé a la machine virtuel
-installation docker desktop.exe
Installation wsl2

Etap2
Sur le projet qu’on a développé avant on va créé un dossier dans notre répertoire et on va le renommé fontend 
On Install notre fontend avec la commande suivante
$ npx create-react-app frontend
Maintenain notre react est instalé et on va instal git dans notre projet  avec la commande  rm –rf .git
Dans le dossier frontend=>src =>app.js pour travaille sur le front end
On Install axios avec la commande$ npm i axios
Maintenant on va crée un fichier dockerfils sur le projet backend et cela pour construire notre image
-on consulte notre image avec la commande : $ docker images
-dans cette étape in va utilisé docker build pour pouvoir accédé a la documentation docker et construite notre images  on utilisant  $docker build . -t projet-alos3
-donc npm Start a était lancé et construit de limage et terminé avec sucée
Pour voir nos image on utilise $docker images
-j’ exécute l’image avec la commande $docker run limage va afficher sur le port http://localhost:3000
<img width="826" alt="Capture" src="https://user-images.githubusercontent.com/98590213/169669829-4959fa3e-420e-4acf-8bc8-ae8f64a19c03.PNG">

Docker compose
Pour le docker compose on va crée un dossier sur visuel code studio DockerCompose et a l’intérieur du dossier on ajout nouveau un fichier docker-compose.yml 
Et cela pour declaré les service donc le cou ou on a besoin que tous les image doit fonctionné ensemble on vas difinir les image la mise a jour au reseaux et les volumele dans le code docker-compose.yml
On lance docker compose avec la commande $ docker-compose up -d
On peux utiliser docker compose pour faire tourner nos conteneurs on peux utiliser la commande $docker-compose down
Mantenain on vas cree un reportoir dur docker hub 
Sur terminal on execute la commande $docker login -u khellaf0886 pour singup
On va etiquter notre emage avecla commande suivante :$ khellaf0886/projet-alos3:latest
Apres on push avec la commande $ docker push khellaf0886/projet-alos3:latest

