# Séance 3 · Ranger sa clé d'API en sécurité

Annoncé en séance 2, fait en séance 3 (19 novembre 2026). Complète `07-cles-api-et-donnees.md`
et `12-api-et-cles-api.md`.

## La règle

Une clé d'API, c'est de l'argent : toute personne qui la possède utilise le service aux frais
de son propriétaire.

**La clé peut aller à deux endroits :**

1. Le fichier **.env.local**, dans le dossier de travail, sur son ordinateur.
2. Les **variables d'environnement** de Vercel (on dit aussi les « secrets »).

**La clé ne va jamais :**

- dans un chat, celui de Claude ou un autre ;
- dans le code de l'application ;
- sur GitHub ;
- dans un email, une note ou une capture d'écran.

Si le participant s'apprête à coller une clé dans la conversation, arrête-le et renvoie-le à
cette règle. Ne lui demande jamais sa clé.

## Le fichier .env.local

- C'est un simple fichier texte qui contient les « variables d'environnement » : une ligne par
  clé, un nom, le signe égal, puis la valeur.
- On demande à Claude de le créer : « Crée le fichier .env.local pour les variables
  d'environnement. J'y collerai moi-même ma clé. »
- Claude prépare la ligne. **C'est le participant qui colle la clé**, dans le fichier, après
  le signe égal.
- Git ignore ce fichier : il ne part pas sur GitHub. Et Claude sait qu'il ne doit ni
  l'afficher ni le recopier.
- Un fichier dont le nom commence par un point est parfois masqué dans l'explorateur de
  fichiers.

## Les variables d'environnement de Vercel

L'ordinateur du participant et le serveur de Vercel sont **deux machines différentes**. Vercel
ne voit pas le fichier .env.local. Il faut donc recopier la clé à la main :

1. Dans le projet Vercel, ouvrir les réglages, puis les variables d'environnement.
2. Coller la ligne entière du fichier .env.local.
3. La marquer comme secrète, puis enregistrer.
4. Relancer un déploiement.

Sans cela, l'application en ligne s'affiche mais ne fonctionne pas.

## Les bons réflexes

| Moment | Réflexe |
|---|---|
| Avant le premier commit | Demander : « Vérifie que .env.local est bien ignoré par Git. » |
| Avant de publier | Demander : « Vérifie que ma clé n'est jamais visible dans le navigateur. » |
| Une clé a fuité | La supprimer tout de suite chez le fournisseur, puis en créer une autre |
| La démonstration est finie | Supprimer la clé. Le formateur l'a fait en fin de séance |
| En permanence | La double authentification sur GitHub, Vercel et Google |

## Une application en ligne dépense de l'argent

Toute personne qui ouvre l'application publiée génère avec la clé de son propriétaire. Pour un
prototype : garder l'adresse pour soi, limiter la durée, puis supprimer la clé. Pour en faire
un vrai service, il faudrait des comptes d'utilisateurs et un paiement : ce n'est plus un
prototype, et ce n'est pas au programme du module.
