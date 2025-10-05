---
description: Veuillez arrêter de me poser les mêmes questions sur le serveur.
---

# ❓ Questions Fréquemment Posées

## Questions

### Pourquoi mes boutons ne s'affichent-ils pas ?

Ceci est un bug Discord. Vous ne pouvez pas voir vos boutons, cependant les autres pourront.

### Est-ce que c'est un virus? Mon antivirus/VirusTotal/etc annonce qu'il y a un virus.

Non. CustomRP ne contient aucun virus, le code source est libremement accessible afin que chacun puisse le vérifier.
No. CustomRP doesn't contain any viruses, the source code is available for everyone to check.

Vous vous demandez peut-être pourquoi certains antivirus et VirusTotal indiquent la présence d’un virus. C’est principalement parce que mon application : 
a) n’est pas assez populaire pour être considérée comme fiable par Windows et certains antivirus. 
b) n’est pas signée avec un certificat de signature de code (étant russe, je ne peux actuellement pas en acheter un, et même si c’était possible, ils sont assez coûteux).

### Puis-je ajouter plus de 2 boutons ?

Non, c'est une limite instaurée par Discord.

### Puis-je utiliser un autre type d'activité (Ex: écoute, regarde, diffuse) ?

Non, c'est aussi une limite instaurée par Discord.

### Pourquoi si je définis un horodatage quelques jours dans le futur, Discord n'affiche que le nombre d'heures restantes ?

Vous l'avez deviné, c'est encore une limite instaurée par Dicord.

### Y aura-t-il une version Linux/MacOS ?

L'application est conçue à l'aide d'une bibliothèque Windows uniquement. Par conséquent, la prise en charge de Linux et MacOS nécessiterait la réécriture de l'ensemble de l'application avec une bibliothèque/langage de programmation différente. Ce que je ne prévois pas pour le moment.

### Une fenêtre appelée "Pipe" s'est ouverte pour une raison quelconque, qu'est-ce que c'est ?

Il s’est ouvert car vous avez appuyé sur Ctrl + Maj et cliqué sur le bouton "Connecter" (ou sur Ctrl + Connecter, ou "Reconnecter" dans le menu de l’icône de la barre d’état dans les anciennes versions). Laissez la valeur à "-1" et fermez la fenêtre. Cette option est utilisée lorsque plusieurs clients Discord sont exécutés simultanément. Modifier le numéro de canal permet de choisir le client dans lequel vous souhaitez que votre présence soit affichée.

## Dépannage

Avant d'essayer quoi que ce soit, assurez-vous d'être sur la dernière version de CustomRP !

### J'ai installé CustomRP mais il ne se lance pas.

Ceci est probablement dû à votre antivirus, qui empêche l’application de se lancer. Ajoutez le dossier `%appdata%\CustomRP` aux exceptions. 

### J'ai installé CustomRP, autorisé les statistiques et l'application ne fonctionne plus.

Fermez l’application via le Gestionnaire des tâches, supprimez le dossier `%localappdata%\maximmax42`, relancez l’application et refusez l’activation des statistiques.

### L'application s'est connectée, mais je ne vois pas l'état dans mon profil

Assurez-vous d'avoir activé le statut d'activité dans les paramètres Discord :

<figure><img src="https://user-images.githubusercontent.com/112771301/196043582-9a04d91f-5c6f-4399-a705-18955e24ea04.png" alt=""><figcaption></figcaption></figure>

Si l’option “Partage ton statut d’activité...” était désactivé, vous devrez aussi activer manuellement le “Statut d’activité” dans les paramètres de confidentialité de chaque serveur comptant plus de 200 membres auquel vous participez.

### L'application fonctionnait, mais maintenant elle se connecte indéfiniment.

Il se peut que Discord vous ait temporairement bloqué à cause de trop nombreuses connexions/changements de présence. Déconnectez-vous, attendez 5 à 10 minutes, puis essayez de vous reconnecter. Redémarrer Discord pourrait aussi aider.

### L'application indique "Mauvaise ID ?"/"Est-ce que Discord est en cours d'exécution ?" ou se connecte indéfiniment même si je suis sûr d'avoir tout fait correctement et que Discord fonctionne.

Voici certaines choses à essayer:

* **Soyez sûr que vous tournez avec le Client Discord (Pas dans un navigateur).**
* Redémarrez votre PC. Conseil : Redémarrer un PC résout beaucoup de problèmes.
* Si vous avez BetterDiscord/Vencord/etc d'installé, désinstallez-les, laissez CustomRP se connecter à Discord au moins une fois, puis réinstallez-le.
* Si vous avez plusieurs clients Discord, quittez-les tous temporairement, sauf celui sur lequel vous souhaitez que la présence soit active.
* Lancez CustomRP en tant qu'Administrateur
* Ajoutez `%appdata%\CustomRP` aux exceptions de votre pare-feu/antivirus. Redémarrez votre PC.
* Au cas où vous utilisez une version portable de CustomRP : Ajoutez le dossier dans lequel vous avez extrait CustomRP aux exceptions de votre pare-feu/antivirus. Redémarrez votre PC.
  * Si vous ne saviez pas si vous avez un antivirus ou non : vous en avez certainement un - Windows Defender est sur tous les ordinateurs avec Windows 10/11
* Réinstallez Discord.

Si rien n'a fonctionné, je ne peux rien faire d'autre, désolé.

### L'application annonce "L'URL de l'image est trop longue" ou l'application est bloquée sur "Mise à jour de la présence..."

Vérifiez l'URL de l'image, ils sont soit
Check the image URLs, they're either too long, or not actually direct links.

### L'application fonctionnait auparavant, mais maintenant elle plante et ne se lance plus du tout.

Vous avez peut-être inséré une longue chaîne de texte sophistiqué (ou du texte dans une langue qui utilise des lettres non latines) dans un champ et cela a planté l'application. Pour résoudre ce problème, appuyez sur Win + R, tapez `%localappdata%\maximmax42` et supprimez ou renommez les dossiers avec CustomRP dans le nom, puis démarrez l'application. Notez que cela réinitialise complètement l'application.

### L'application n'arrête pas de planter lors de la mise à jour/tentative de connexion/etc.

Si vous parvenez à lancer l'application et à obtenir un rapport de plantage, et qu'il indique `System.IO.FileNotFoundException: Could not load file or assembly...`, veuillez réinstaller l'application.

Si vous ne trouvez pas de réponse à votre question/problème, envoyez un message au salon `#support` sur le [serveur Discord de CustomRP](https://www.customrp.xyz/discordserver) ou bien envoyez un message à maximmax42 sur Discord ou [Ouvrir un Issue](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
