1- Télécharger Java SE developpement Kit 
http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html
2- installer jdk 
3- Télécharger android sdk 
http://developer.android.com/sdk/index.html#Other
4- installer sdk 
copier Dans votre variable d'environnement PATH 
C:\Users\IAB3491.VISEO\AppData\Local\Android\android-sdk\platform-tools
5- Installer node
https://nodejs.org/en/
6- installer cordova et ionic 
npm install -g cordova ionic
7- dans votre repertoir du projet 
 ionic start non_project
8- ionic serve (pour lancer l'app dans le navigateur)
9- sinon pour le build 
 9-1 ajouter la platorm cible 
     pour android : ionic platform add android
     pour ios ; ionic platform add ios
 9-2 build 
     ionic build anroid (Apk non signé)
     ionic build android -- release (Apk mode non debug) ensuite 
     ionic build ios (project.xcodeproject) ensuite on build une Ipa (besoin de compte developpeur IOS)
  


