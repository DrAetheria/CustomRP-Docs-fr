---
description: Lisez le putain de manuel. (Bordel.)
---













# 🛠️ Mise en Place

Si vous rencontrez des erreurs, consultez [FAQ](faq.md).

Avant la configuration, assurez-vous d'avoir le Client Discord (**Et non sur Navigateur**) et d'avoir activé le statut d'activité dans les paramètres Discord:

<figure><img src="https://user-images.githubusercontent.com/112771301/196043582-9a04d91f-5c6f-4399-a705-18955e24ea04.png" alt=""><figcaption></figcaption></figure>

Si l’option “Partage ton statut d’activité...” était désactivé, vous devrez aussi activer manuellement le “Statut d’activité” dans les paramètres de confidentialité de chaque serveur comptant plus de 200 membres auquel vous participez.

## Procédure de Mise en Place

* Aller sur [Discord Developer portal](https://discord.com/developers/applications). (Le site n'est pas en français.)
* Cliquer **New Application** en haut à droite.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Choisir un nom pour l'application, il sera affiché après "En train de jouer" dans le statut ; appuyez sur **Create**.
* Copiez **l'ID d'application (Application ID)** et collez-le dans le logiciel CustomRP dans la partie **ID**, puis appuyez sur **Connecter**. 

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

*Si cela est fait correctement, votre statut dans Discord devrait maintenant indiquer "En train de jouer **\[nom de l'application]**". Au cas ou vous encontrez des erreurs: voir la [FAQ](faq.md).
  *Le statut ne se montrera pas si vous êtes en mode invisible.
  *Si vous avez un statut customisé en marche (Celui avec l'emoji), il sera prioritisé sur le statut CustomRP. Cependant le statut CustomRP sera vu sur le popup du profil.

*Vous pouvez désormais remplir les autres champs. (Tout sauf "Type" est optionel):
  * **Type**: Le type de présence.
    * Utiliser tout autre type que "Playing" désactive le "Party count".  Les "Types" concurrents désactivent également les horodatages.
  * **Details**: Première ligne de la présence sous le nom de l'application.
  * **State**: Deuxième ligne de la présence. Sera premier si le champ "Details" est vide.
  * **Party**: S'affiche en tant que `(X of Y)` après la ligne "State".



    * If State is empty, Party count will not be shown on mobile, but will on PC. If both Party and State are present, they'll show at the bottom of the presence on PC.
  * **Timestamp**: A timer that counts from a specific timestamp. Displayed below Details and State as `(hh:)mm:ss`.
  * **Big and small images**: Images that are shown on the left side of the presence. If both are present, small image is in the bottom right corner of the big one.
    * **Key**: Either a direct URL (preferred, as you can also use GIFs that way) or an Art Asset name.
      * _URL method:_ If your image is already on the internet, put the **direct link** (usually done by right clicking the image and choosing something like "Copy image link") in the field. If your image is on your PC, use any image hosting and sharing website (e.g. Imgur, ImageShack, etc). It's **not recommended** to upload images sent in Discord DMs/channels, as their links get too big too quickly and they expire in 2 weeks.
        * If after connecting you get stuck on "Updating presence...", chances are the URL you've put was too long or was not a direct URL. If you're sure it's a direct one, use a URL shortner.
      * _Art Asset method:_ On your application's page, navigate to Rich Presence -> Art Assets and upload at least one image under Rich Presence Assets. In CustomRP, there is a handy **Upload Assets** button in File menu (you can also use Ctrl+U) that will take you there if your ID field is set up properly.
        * Note 1: Although usually the images become usable instantly, in some cases it might take up to several hours.
        * Note 2: While you can name your asset with any name up to 999 symbols, the app will only accept names with 256 symbols max.
    * **Text**: A text that appears when you hover over (or long tap on mobile) the image.
  * **Buttons**: ⚠ Please note, there is currently a Discord bug - you can't see your own buttons, but others will see them.
    * **Text**: A text displayed on the button.
    * **URL**: A URL that the button will open upon clicking.
* Hit **Update Presence** (or **Connect** if you aren't already connected).
* Congratulations, you're wonderful!


























  
* Sur la page de votre application, accédez à Rich Presence -> Art Assets et téléchargez au moins une image sous Rich Presence Assets si vous souhaitez les utiliser. Dans CustomRP, il existe un bouton pratique \*\* Télécharger les ressources \*\* dans le menu Fichier (vous pouvez également utiliser Ctrl + U) qui vous y mènera si votre champ ID est correctement configuré.
  * Alternativement, vous pouvez simplement insérer une URL vers l'image dans le champ **Clé**.
  * Remarque : Bien que vous puissiez nommer votre élément avec n'importe quel nom jusqu'à 999 symboles, l'API n'accepte que les noms contenant 256 symboles au maximum.
* Accédez à la page Visualizer pour configurer les champs \*\* État, Détails, Grande clé d'image, Texte de grande image, Petite clé d'image, Petit texte d'image, Taille de la fête, Party Max \*\*. Tous ces éléments sont facultatifs.
* Une fois que vous avez trouvé la configuration qui vous convient, copiez les valeurs dans les champs correspondants de CustomRP.
  * Conseil : Vous pouvez survoler presque n'importe quel contrôle de l'application (y compris la ligne d'étiquettes **Détails**) et une info-bulle s'affichera !
* Si vous souhaitez également configurer des boutons, remplissez les champs Texte et URL.
  * Remarque : Lorsque vous cliquerez sur les boutons en votre propre présence, ils ne fonctionneront pas, mais ne vous inquiétez pas, ils fonctionneront pour tout le monde. C'est un problème du côté de Discord.
* Appuyez sur **Mettre à jour la présence** (ou **Connecter** si vous n'êtes pas déjà connecté).
* Félicitations, vous êtes merveilleux !

### J'utilise plus d'un client Discord, que dois-je faire ?

Si vous avez plus d'un client Discord et que vous souhaitez que votre présence apparaisse sur un compte différent de l'application choisie automatiquement, veuillez appuyer sur **Déconnecter**, puis maintenez les touches Ctrl+Maj de votre clavier et appuyez sur \*_Connecter_ \*. Une fenêtre avec une entrée de nombre apparaîtra, mettez un nombre 1, fermez la fenêtre et appuyez à nouveau sur **Connecter**, sans Ctrl+Maj. Au cas où il s'agirait encore d'un mauvais compte, essayez le numéro 0, puis le 2 et ainsi de suite jusqu'au 9.

Veuillez noter que si vous avez plusieurs clients Discord exécutés au démarrage, le numéro de canal attribué à chaque client peut ne pas être persistant d'un démarrage à l'autre et peut changer en fonction du client démarré en premier. Pour éviter cela, vous pouvez soit démarrer manuellement des clients supplémentaires, soit utiliser le planificateur de tâches Windows pour retarder le démarrage des clients.

Si vous avez 2 comptes que vous utilisez en même temps et que vous souhaitez que chacun d'eux ait une présence différente, suivez ces étapes :

* Commencez par configurer votre compte principal en suivant les instructions ci-dessus.
* Procurez-vous la dernière version **portable (.zip)** de CustomRP (soit depuis le [site](https://www.customrp.xyz) ou sur [Page des versions de GitHub](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) et déballez-le n'importe où.
  * Ceci fonctionne seulement avec les versions 1.16 et plus.
* Ouvrez `Start Second Instance.bat` ou créez un raccourci vers CustomRP.exe avec un argument `--second-instance` (ou `-2`).
* Configurez le programme de la même manière que vous l'avez fait pour votre instance principale.
  * Conseil : Si vous disposez déjà d'un préréglage que vous souhaitez utiliser avec votre deuxième instance, vous pouvez modifier le fichier bat ou le raccourci pour inclure le chemin d'accès au préréglage. Exemple : `CustomRP.exe -2 "C:\Some Folder\preset.crp"` (des guillemets autour du chemin sont nécessaires si le chemin contient des espaces).
* Avant le raccordement, changez le tuyau comme décrit précédemment et raccordez.

Si vous utilisez 3 comptes ou plus en même temps, alors... pourquoi ? Mais aussi, si vous êtes assez nombreux à me harceler, j'ajouterai un support pour utiliser plus d'instances.

## Notes

* Si vous ne souhaitez pas configurer une petite ou une grande image, laissez tous les champs associés vides dans le programme.
* Si la grande image n'est pas définie, les paramètres de la petite image seront ignorés.
