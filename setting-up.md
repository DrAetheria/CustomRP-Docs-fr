---
description: RTFM
---

# 🛠 Mise en Place

Si vous rencontrez des erreurs, consultez [FAQ](faq.md).

Avant la configuration, assurez-vous d'avoir activé le statut d'activité dans les paramètres Discord:&#x20;

<figure><img src="https://user-images.githubusercontent.com/112771301/196043582-9a04d91f-5c6f-4399-a705-18955e24ea04.png" alt=""><figcaption></figcaption></figure>

## Procédure de Mise en Place

* Aller sur https://discord.com/developers/applications/. (Le site n'est pas en français.)
* Cliquer **New Application** en haut à droite.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Choisir un nom pour l'application, il sera affiché après "En train de jouer" dans le statut ; appuyez sur **Create**.
* Copiez **l'ID d'application (APPLICATION ID)** et collez-le dans le logiciel CustomRP dans **ID**, puis appuyez sur **Connecter**. Si cela est fait correctement, votre statut dans Discord devrait maintenant indiquer "En train de jouer **\[nom de l'application]**".
  * Remarque : Si vous avez défini un statut personnalisé (celui avec emoji), il sera prioritaire par rapport à celui de votre CustomRP. Il sera cependant visible dans la fenêtre contextuelle du profil.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Sur la page de votre application, accédez à Rich Presence -> Art Assets et téléchargez au moins une image sous Rich Presence Assets si vous souhaitez les utiliser. Dans CustomRP, il existe un bouton pratique ** Télécharger les ressources ** dans le menu Fichier (vous pouvez également utiliser Ctrl + U) qui vous y mènera si votre champ ID est correctement configuré.
  * Alternativement, vous pouvez simplement insérer une URL vers l'image dans le champ **Clé**.
  * Remarque : Bien que vous puissiez nommer votre élément avec n'importe quel nom jusqu'à 999 symboles, l'API n'accepte que les noms contenant 256 symboles au maximum.
* Accédez à la page Visualizer pour configurer les champs ** État, Détails, Grande clé d'image, Texte de grande image, Petite clé d'image, Petit texte d'image, Taille de la fête, Party Max **. Tous ces éléments sont facultatifs.
* Une fois que vous avez trouvé la configuration qui vous convient, copiez les valeurs dans les champs correspondants de CustomRP.
  * Conseil : Vous pouvez survoler presque n'importe quel contrôle de l'application (y compris la ligne d'étiquettes **Détails**) et une info-bulle s'affichera !
* Si vous souhaitez également configurer des boutons, remplissez les champs Texte et URL.
  * Remarque : Lorsque vous cliquerez sur les boutons en votre propre présence, ils ne fonctionneront pas, mais ne vous inquiétez pas, ils fonctionneront pour tout le monde. C'est un problème du côté de Discord.
* Appuyez sur **Mettre à jour la présence** (ou **Connecter** si vous n'êtes pas déjà connecté).
* Félicitations, vous êtes merveilleux !

### J'utilise plus d'un client Discord, que dois-je faire ?

Si vous avez plus d'un client Discord et que vous souhaitez que votre présence apparaisse sur un compte différent de l'application choisie automatiquement, veuillez appuyer sur **Déconnecter**, puis maintenez les touches Ctrl+Maj de votre clavier et appuyez sur **Connecter* *. Une fenêtre avec une entrée de nombre apparaîtra, mettez un nombre 1, fermez la fenêtre et appuyez à nouveau sur **Connecter**, sans Ctrl+Maj. Au cas où il s'agirait encore d'un mauvais compte, essayez le numéro 0, puis le 2 et ainsi de suite jusqu'au 9.

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
