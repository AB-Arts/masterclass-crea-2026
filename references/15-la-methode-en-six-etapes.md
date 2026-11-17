# La méthode en six étapes (séance 2, partie 2)

Des participants ont demandé un mode d'emploi : « au tout début, on fait quoi, on lui dit
quoi ? ». Le formateur a dicté les étapes lentement. Les voici. C'est **la** marche à suivre du
module.

## Les six étapes

1. **Ouvrir Claude Desktop en mode Code.** Pas le mode Chat.
2. **Créer une conversation et choisir un dossier** de son ordinateur. Tout ce qui sera créé
   s'y enregistre.
3. **Créer un nouveau dépôt sur GitHub**, en **privé**, et copier son lien.
4. **Coller ce lien dans la conversation** et dire : « Voici le dépôt dans lequel tu vas
   versionner ce qu'on fait dans ce dossier. »
5. **Construire.** Décrire ce qu'on veut, regarder l'aperçu à droite, corriger. De temps en
   temps : « commit sur le Git ».
6. **Quand on veut le montrer en ligne** : créer un projet sur Vercel, importer le dépôt,
   déployer. On obtient une adresse web. Voir `13-vercel-mettre-en-ligne.md`.

Pourquoi le dépôt en plus du dossier : sur l'ordinateur, Claude écrase les fichiers, on n'a
que la dernière version. GitHub garde toutes les autres.

## L'ordre compte

Trois erreurs vues en séance :

- **Vouloir pousser sur GitHub ou sur Vercel avant d'avoir créé quelque chose.** Il n'y a rien
  à envoyer. D'abord un dossier, puis quelque chose dedans, puis le commit, puis Vercel.
- **Être en mode Chat au lieu du mode Code.** Vérifier en haut de la fenêtre.
- **Confondre son dépôt et celui du formateur.** Votre dépôt reçoit votre projet. Le dépôt du
  formateur est un exemple à consulter ; pour vous en servir, donnez son lien à Claude et
  demandez-lui de **copier le code dans votre propre dépôt**.

## Vérifier où l'on est

- **Le dossier de travail** : son nom s'affiche dans la conversation. En cliquant dessus, on
  peut l'ouvrir dans l'explorateur de fichiers.
- **Le lien du dépôt** : sur la page du dépôt GitHub, un petit bouton permet de le copier. Sur
  GitHub, la dernière version est toujours la version principale.
- **Si un premier travail existe déjà sans dépôt** : créer le dépôt, coller son lien dans la
  conversation du projet, et dire « commit sur ce Git ». La première version apparaît.
- **Le modèle** : à chaque nouvelle conversation, regarder quel modèle est sélectionné. Le
  formateur a ouvert un chat qui s'était mis tout seul sur le modèle le plus cher, à l'effort
  maximum.

## Autoriser Claude sur GitHub

Si, à l'import d'un dépôt, Vercel ou Claude demande d'**installer l'application GitHub** :
accepter, autoriser tous les dépôts, valider avec le code reçu par email, puis cliquer sur
**Connect**. Ne pas aller trop vite : chaque écran compte.

## Il n'y a pas de mode d'emploi, et c'est voulu

Le formateur l'a dit clairement : le vrai mode d'emploi, **c'est de demander à Claude**.

> Je veux faire du prototypage. J'utilise tel logiciel. J'ai un compte GitHub et un compte
> Vercel. Je veux faire ceci. Dis-moi quoi faire.

Et quand on ne comprend pas :

> Je suis débutant. Explique-moi comme à un enfant, étape par étape, ce que je dois faire.

Il le fait lui-même tous les jours. On peut aussi envoyer une capture d'écran et demander où
cliquer.

## Pourquoi on ne pratique pas longuement pendant la séance

Trois heures en visio, c'est court. Si le formateur reste une heure sur le blocage d'une
personne, les autres n'apprennent rien. Il envoie donc de l'information, la regroupe dans les
documents et dans cette skill, et répond aux questions. La pratique se fait **entre les
séances**. Un devoir est annoncé pour la dernière séance.

## Apporter un cas

Demande répétée du formateur : pour qu'il puisse travailler sur du concret, **envoyez-lui un
cas** tiré de votre métier. Passez par CREA, qui transmet. Un cas, c'est : ce qui entre, ce
qui doit sortir, et ce que vous faites aujourd'hui à la main entre les deux.

## Ce qu'on peut déjà faire

- Construire une petite application en local et la publier en ligne.
- Un petit site pour la famille ou pour une idée.
- **Pas de données sensibles.** Uniquement du prototypage et des tests.
