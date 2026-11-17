# Séance 2, partie 1 : les rappels et ce qui a été précisé

La séance 2 (mardi 17 novembre 2026) a commencé par une relecture du récapitulatif de la
séance 1. Ce fichier ne répète pas la séance 1 : il contient ce qui a été **ajouté ou précisé**.

## Deux documents par séance

Pour chaque séance, il y a deux PDF :

- le **plan de séance**, préparé avant : ce qui était prévu ;
- le **récapitulatif**, écrit après : ce qui a vraiment été vu, avec les remarques et les
  différences par rapport au plan.

Ils sont diffusés par CREA sur la plateforme du cycle. S'il en manque un, le demander à CREA.

## Le fichier .md, la langue commune des modèles

Un fichier `.md` est du simple texte. C'est le format que **tous les modèles** lisent le
mieux : il passe de Claude à ChatGPT ou à Gemini sans rien changer. C'est pour cela que la
mémoire d'un projet se range dans des fichiers `.md`, sur l'ordinateur ou sur GitHub.

## Récupérer une conversation du mode Chat : le handover

Le mode Chat sert aux discussions du quotidien, celles qu'on n'a pas besoin de garder. On peut
même y **parler à voix haute**, par exemple en voiture, ce que le mode Code ne permet pas.

Mais parfois une discussion devient intéressante et on veut en faire quelque chose. Dans ce
cas, on demande à la fin :

> Fais un handover en .md de ce chat.

Claude produit un fichier `.md` à télécharger. On le dépose dans un dossier de travail, on
ouvre ce dossier en mode Code, et on continue à partir de là. Le fichier peut aussi être donné
à une autre IA.

Exemple du formateur : une discussion sur la réparation d'une toiture qui devient l'idée d'un
générateur d'offres pour réparer des toitures.

## Un chat, une idée, un fichier

Astuce donnée pour les débutants : **saucissonner avec le mode Chat**.

- Un chat pour les camemberts des ventes. Quand la solution vous plaît : handover en `.md`.
- Un autre chat pour l'affichage du chiffre d'affaires et du résultat : handover en `.md`.
- Et ainsi de suite.

À la fin, le dossier de travail contient un fichier par tranche. C'est une base de travail et
un historique durable.

## L'affinage

**Affiner**, c'est travailler une idée avec l'IA jusqu'à ce qu'elle ait compris exactement le
besoin et qu'elle y réponde vraiment, avec ou sans documentation extérieure. On ne demande le
handover qu'une fois l'idée affinée.

## Conditionner l'IA, ne pas se laisser conditionner

Le formateur y a insisté. Plus on utilise ces outils, plus l'IA propose des solutions. Le
risque est de finir par fonctionner selon ce que l'IA propose, et plus selon son propre savoir.

- **C'est vous qui conditionnez l'IA à votre besoin**, pas l'inverse.
- Il faut plus que jamais **connaître les fondamentaux** de son métier, vérifier, et comprendre
  d'où vient un résultat.
- Si on perd le contrôle, l'outil devient moins bon, et nous aussi.

## Le front et le back

- Le **front** (*front end*) : ce que l'on voit et ce que l'on utilise. Les boutons, les
  textes, les écrans. Dans une messagerie, ce sont les bulles et les icônes.
- Le **back** (*back end*) : ce que l'on ne voit pas. Le code, les calculs, le stockage.

Dans Claude, **l'artefact montre le front**, et l'onglet de code montre le back. Un designer
fait du front. Une clé d'API, c'est du back. Un bouton rose en haut à droite, c'est du front.

## La stack, avec l'image de la maison

La **stack** est l'architecture du back : l'ensemble des fournisseurs choisis.

Exemple d'un site de vente de bijoux. Il faut décider :

- où ranger le code (GitHub) ;
- qui met le site en ligne et le relie à un nom de domaine (Vercel) ;
- où ranger les données des clients et des commandes (une base de données, par exemple
  Supabase) ;
- où ranger les photos (un stockage, par exemple Cloudflare) ;
- qui encaisse les paiements (par exemple Stripe).

L'image : **construire une maison**. Il faut toujours des briques, des portes, des fenêtres,
une charpente, mais ils viennent de fournisseurs différents. L'ensemble des fournisseurs, c'est
la stack. La maison finie, avec ses poignées, c'est le front. Ce qui passe dans les murs et les
fondations, c'est le back. Il existe une infinité de combinaisons possibles.

## Les modèles : ce qui a été précisé

Voir aussi `03-modeles-tokens-abonnements.md`. Les précisions du 17 novembre :

- **Haiku** : parfait pour appliquer une skill écrite par un modèle plus fort. Mauvais choix
  pour développer quelque chose.
- **Sonnet** : léger aussi, mais capable d'écrire à votre façon, de manière plus humaine.
- **Opus** : l'outil pour développer des applications. Il existe en plusieurs versions ; plus
  la version est récente, plus elle est intelligente et plus elle coûte.
- **Fable** : pour les réflexions et analyses très profondes, le storytelling, un gros premier
  jet sur un dossier énorme. Inutile pour une application, un tableau de bord ou des calculs
  courants. Pas disponible avec la formule à 20 par mois.
- **L'effort** : moyen, élevé, puis des niveaux encore plus hauts. Chaque cran consomme
  nettement plus. Le réglage du formateur neuf fois sur dix : **Opus récent, effort moyen**.
  « Ça passe partout. »
- **Quand le quota est vide**, il faut attendre la fenêtre suivante (environ quatre heures)
  avant de pouvoir continuer.
- **Deux compteurs** : la consommation de Fable est comptée à part de celle des autres
  modèles. On peut avoir épuisé Fable et continuer avec Opus.
- **Le joker** : selon le formateur, un nouvel abonné peut réinitialiser gratuitement sa
  consommation une fois (Paramètres, Utilisation). Son conseil si vous ne prenez l'abonnement
  qu'un mois : consommez tout, puis utilisez le joker. À vérifier dans votre compte.

Le but reste le même : construire le plus vite possible des outils qui tournent seuls, pour
limiter la consommation de tokens.
