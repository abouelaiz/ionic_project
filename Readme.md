## Installation environnement ionic 



1. Télécharger et installer Java SE developpement Kit 

   http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html.

2. Télécharger et installer  android sdk

http://developer.android.com/sdk/index.html#Other.
lors de l'installation il faut  copier install location  par exemple pour moi c'etait "C:\Users\IAB3491.VISEO\AppData\Local\Android\android-sdk\".
 ![alt text](https://github.com/abouelaiz/ionic_project/blob/master/install.PNG "Logo Title Text 1")

4. And another item

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

⋅⋅⋅ ensuite vous concatener \platform-tools a votre location vous devez avoir a la fin vous aurez quelque chose comme 
⋅⋅⋅"C:\Users\IAB3491.VISEO\AppData\Local\Android\android-sdk\platform-tools"

⋅⋅⋅copier Dans votre variable d'environnement PATH .
5. Installer node.
...https://nodejs.org/en/
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