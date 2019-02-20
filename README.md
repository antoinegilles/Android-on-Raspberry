# Mise en place d’un OS Android sur Raspberry


![picture](https://user-images.githubusercontent.com/35256402/53077457-54be5300-34f2-11e9-8769-a4fe12361415.jpg)

### 1 – Installer l’OS Android

Pour cette étape il suffit de suivre les étapes expliquer sur ce site dans la partie « Installation d’Android sur la carte SD » : https://raspbian-france.fr/installer-android-raspberry-pi/ . L’étape est assez simple : 
-	Munissez-vous d’une carte SD
-	Télécharger l’image Android ( sur le site )
-	Télécharger Etcher qui vous permettra de « flasher » installer l’image téléchargé sur la carte SD

Voilà, vous avez installé une image Android sur votre Raspberry !

### 2 – Installer le Play Store

De même vous allez pouvoir suivre les informations du tutoriel sur le même lien dans la partie « Installation du Play Store ». 
-	Installer le script sh ( il va permettre de télécharger les ressources pour le Play Store )
-	Pour l’étape « sudo apt install android-tools-adb » vous devrez utiliser une machine linux . De plus vous connectez faite attention a ce que votre Wi-Fi ne restreint pas les connexions SSH ( pour ma part j’ ai utilisé le partage de connexion de mon smartphone )
-	Enfin, avant de réaliser la dernière étape du tutoriel , il est important de changer une ligne de code dans le script « sh » :
A la ligne 24 du script , TIMESTAMP vaut « 20171022 », Cette version est périmé.
Il va falloir changer cette version selon la bibliothèque suivante : https://github.com/opengapps/arm/releases Choisissez la bonne année ( Aujourd‘hui j’ai choisi 20190209 qui est la dernière Realease).


![code](https://user-images.githubusercontent.com/35256402/53083472-49bdef80-34ff-11e9-844b-706cbb0c042c.png)

-	Exécutez les dernière ligne de commande et le script dezipera le dossier téléchargé et installera le Play Store sur votre Raspberry. 



Voilà !  Vous avez maintenant un Raspberry avec un OS Android et le Playstore.


![android2](https://user-images.githubusercontent.com/35256402/53083715-b89b4880-34ff-11e9-8b20-13bd0279304a.png)


Documentation présenté par Antoine Gilles. Remerciement à Raspbian-France.fr.

