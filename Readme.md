# Guide d'installation ionic project
##  Qu’est-ce que Ionic Framework ?

 Ionic Framework est un mélange d’outils et de technos pour développer des applications mobiles hybrides rapidement et facilement. Il s’appuie sur AngularJS pour la partie application web du framework et sur Cordova  pour la partie construction des applications natives. 
##  Comment on procéde créer un projet ionic ? 
1. Pour générer une application mobile hybride, il vous faut le SDK Java et le SDK Android c'est pourquoi je vous invite à:

     Télécharger et installer Java SE developpement Kit    [lien de téléchargement](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html) 
     
    Télécharger et installer android sdk   [lien de téléchargement](http://developer.android.com/sdk/index.html#Othe), 
    il faut juste ne pas oublier d'ajouter les variables d’environnement de système.
    
    Pour windows :
    ```cmd
     set ANDROID_HOME=C:\<installation location>\android-sdk-windows
     set PATH=%PATH%;%ANDROID_HOME%\tools;%ANDROID_HOME%\platform-tools
    ```
     Pour Mac :
    ```cmd
     export ANDROID_HOME=/<installation location>/android-sdk-macosx
     export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools
    ```
    
    
2. Ensuite la deuxiéme chose a faire c'est de télécharger et installer Nodejs pour la simple raison c'est que ionic a besoin de npm pour  installer et gérer les dépendances entre les modules dont il a besoin  . 
    [lien de téléchargement](https://nodejs.org/en/)
3. installer ionic et cordova 
    ```cmd
     npm install -g cordova ionic
    ```
4. créer votre projet ionic 
    ```javascript
    //blank pour un projet vide 
     ionic start Garagiste blank
    ```
   
5. Pour simuler notre application dans le navigateur 
   ```cmd
    ionic serve
    ```
    une autre commande utilisé pour simulé dans le navigateur
   ```cmd
    ionic serve --lab
    ```
   avec cette commande a quoi ressemblerai notre app sur Android et IOS 
6. Enfin on est arrivé  au  build   de l'application  
   on commence par ajouter notre platforme cible
    ```cmd
    // pour android
    ionic platform add android
    // pour IOS
    ionic platform add ios
    ```
    esuite on build notre application pour la platform cible
    ```cmd
    // pour android (on récupére un Apk non signé)
     ionic build anroid 
    // pour IOS (on récupére un xcodeproject)
     ionic build IOS
    ```    
    
      ionic build ios (project.xcodeproject) ensuite on build une Ipa (besoin de compte developpeur IOS)