# Séance 3 · L'exercice : un petit studio de génération, pas à pas

Construit en direct le 19 novembre 2026, puis dicté par le formateur comme marche à suivre.
C'est aussi le devoir proposé pour la séance 4 (voir `09-suite-du-module.md`).

L'application de la séance s'appelle « Rosée Studio ». Elle a un thème clair et un thème
sombre, et s'adapte au téléphone. Des captures d'écran figurent dans le récapitulatif PDF de
la séance 3.

L'application : une zone de texte où l'on demande ce que l'on veut générer, la dictée à la
voix, et en dessous une image, un son ou une vidéo selon la demande.

## La stack de l'exercice

| L'outil | Son rôle | Ce qu'il contient |
|---|---|---|
| Claude Code | Il construit l'application | Rien : il écrit dans le dossier |
| Claude Design | Il dessine l'apparence, à part | La charte, remise dans le dossier .design |
| Le dossier de travail | Il garde tout sur l'ordinateur | Le code, la charte, et la clé dans .env.local |
| GitHub | Il garde les versions | Le code et la charte. Jamais la clé |
| Vercel | Il met en ligne | L'application publiée, et la clé dans ses variables d'environnement |
| Google AI Studio | Il fabrique les images, les sons, les vidéos | Les modèles, et la facture |

Le chemin du code : dossier, puis GitHub (commit), puis Vercel. Le chemin de la clé : elle
reste dans .env.local sur l'ordinateur, et on la recopie à la main dans Vercel.

## Les treize étapes

1. **Créer un dossier** sur son ordinateur, et copier son chemin.
2. **Ouvrir Claude en mode Code**, créer une conversation et un environnement, et le relier à
   ce dossier.
3. **Décrire l'application** : « Fais une application React avec une zone de texte où je
   demande ce que je veux générer. Je dois pouvoir dicter ma demande à la voix. En dessous, le
   résultat s'affiche selon la demande : une image, un son ou une vidéo. »
4. **Dessiner l'apparence avec Claude Design**, dans un autre onglet : décrire la même
   application et le style voulu. En séance : du rose, des apparitions lentes, des particules.
5. **Faire le handoff du design** : créer un dossier `.design` dans le dossier de travail,
   puis demander « Fais un handoff de l'entièreté du design dans le dossier .design de mon
   dossier de travail. »
6. **Faire créer le fichier .env.local** dans la conversation de code (voir
   `18-ranger-sa-cle-api.md`).
7. **Créer la clé dans Google AI Studio** : aistudio.google.com, la petite clé en bas à
   gauche, régler le moyen de paiement si besoin, puis « Create API key » en haut à droite.
8. **Coller la clé dans .env.local**, après le signe égal, et enregistrer. Nulle part ailleurs.
   Dans l'application de la séance, la ligne s'appelle `GEMINI_API_KEY=`. Le nom exact est
   celui que Claude a prévu dans le fichier.
9. **Créer un dépôt privé sur GitHub**, donner son lien à Claude : « Voici le dépôt du projet.
   Vérifie que .env.local est ignoré par Git, puis commit. »
10. **Tester sur son ordinateur** : l'application s'ouvre dans l'aperçu, à une adresse qui
    commence par localhost. Si le micro est refusé, copier cette adresse dans son navigateur
    habituel et autoriser le micro.
11. **Corriger, puis commit** : dire ce qui ne va pas. En séance : un rond resté au milieu de
    l'écran, un lecteur audio où l'on ne pouvait pas avancer.
12. **Mettre en ligne sur Vercel** : nouveau projet, importer le dépôt, « Déployer ».
    L'application s'affiche mais ne génère rien : la clé n'y est pas encore.
13. **Recopier la clé dans les variables d'environnement de Vercel**, la marquer comme
    secrète, puis redéployer.

Sans Claude Design, on passe les étapes 4 et 5 et on décrit le style dans la conversation de
code.

## Pourquoi un design à part

Le code et l'apparence sont deux travaux. En les séparant, on peut refaire le style sans
toucher au reste, et réutiliser la même charte pour un autre outil ou pour ses documents (des
offres qui ont toujours le même visage, par exemple).

## Ce que le test a montré

- **Rien n'est gardé.** En rechargeant la page, les générations ont disparu : il n'y a pas de
  base de données. Pour garder des résultats ou créer des comptes, il en faut une.
- **La base de données** : le formateur utilise Supabase. Elle se relie à Claude en ligne de
  commande, comme GitHub : « Je vais créer une base de données Supabase », puis on suit les
  étapes. On choisit la région des serveurs à la création du projet. Ce n'est pas au programme
  du module : n'en fais pas un tutoriel.
- **En local** veut dire sur son ordinateur : l'adresse en localhost n'est visible que de soi.
- **Les coûts** : voir `17-google-ai-studio-et-vertex.md`.

## Dépannage

**L'application en ligne s'affiche mais ne génère rien.**
La clé n'est pas dans les variables d'environnement de Vercel, ou le projet n'a pas été
redéployé après l'ajout.

**Le micro ne marche pas dans l'aperçu.**
Ouvrir l'adresse localhost dans son navigateur habituel et autoriser le micro.

**Je ne vois pas le fichier .env.local ou le dossier .design.**
Les éléments dont le nom commence par un point sont parfois masqués. Demander à Claude de
l'ouvrir, ou afficher les éléments masqués dans l'explorateur.

**J'ai collé ma clé dans le chat par erreur.**
La supprimer tout de suite dans Google AI Studio et en créer une autre.
