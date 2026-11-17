# Les API et les clés d'API, plus en détail (séance 2, partie 1)

Complète `07-cles-api-et-donnees.md`. La règle ne change pas : **jamais de clé d'API dans un
chat**, jamais dans un dépôt public.

## L'API et la clé d'API

- Une **API** est l'interface qu'un service met à disposition pour que d'autres applications
  puissent l'utiliser. Le « I » veut dire *interface*.
- La **clé d'API** est ce qui donne accès à cette interface.

L'image : **une porte avec une serrure**. L'API est la pièce derrière la porte. La clé d'API
ouvre la porte.

Aujourd'hui, presque tous les outils en ligne un peu professionnels ont une connexion par API.

## Une clé n'ouvre pas forcément tout

Imaginez une pièce fermée à clé qui s'appelle Google Maps. Dedans : un four à micro-ondes, des
toilettes et une douche. On peut fabriquer une clé qui ouvre la porte **mais ne permet
d'utiliser que la douche**.

Quand on crée une clé d'API, on choisit donc les fonctions qu'elle autorise. Exemple : pour un
site de bijoux, la clé Google Maps sert seulement à afficher la carte et la position du
magasin. Pas la recherche, pas la vérification d'adresses.

Autre image proposée par un participant et validée par le formateur : un raccord entre le
robinet du jardin et le système d'arrosage. Sans la clé, l'eau ne passe pas.

## Ce que ça coûte

Chaque fournisseur a son prix **à l'appel** (en anglais *call*). Il y a souvent un volume
gratuit, puis un tout petit prix par appel supplémentaire. Le coût dépend donc de l'usage :
quelles fonctions, et combien de fois. C'est ainsi que ces entreprises se rémunèrent.

## Où on les trouve

Le formateur a montré la console Google Cloud (rubrique des API et services) : des centaines
d'API à activer ou désactiver. Cartes, traduction, agenda, tableur, YouTube, etc. On retrouve
la même logique chez les autres grands fournisseurs et chez les services de paiement.

Question posée : est-ce payant d'y accéder ? Un compte Google suffit normalement pour ouvrir la
console ; c'est l'usage des API qui peut devenir payant.

## Pourquoi une clé est sensible

Une clé qui traîne (collée dans un chat, laissée dans un dépôt public) peut être récupérée par
une personne ou un robot, qui utilisera le service **à vos frais**.

**Une sécurité supplémentaire** : on peut limiter une clé à un **nom de domaine**. La clé ne
fonctionne alors que depuis votre site. Si elle est volée, elle ne sert à rien ailleurs.

## Où range-t-on la clé, alors ?

Question posée : « on génère la clé, puis on la met sur notre site ? » Non. On ne la met pas
dans le site. Deux endroits prévus pour cela, annoncés en séance 2 puis **reportés à la
séance 3** :

- les **secrets** (chez Vercel : les *variables d'environnement*) : l'endroit sécurisé où une
  application en ligne garde ses clés ;
- les **fichiers d'environnement locaux** : un fichier sur votre ordinateur qui garde les clés
  sans les envoyer sur GitHub ni les publier.

Le détail pratique sera vu en séance 3. D'ici là, n'explique pas la manipulation : dis que
c'est au programme et propose de noter la question pour Anthony.

Autre précaution donnée en séance 2 : quand on branche un outil sur de vraies données, on
demande une clé **en lecture seule**. Voir `14-vraies-donnees-limites-et-exemples.md`.

## CLI, MCP, API : la précision du 17 novembre

Ce sont trois **tunnels de communication** sécurisés entre deux outils :

| Tunnel | En simple | Exemple |
|---|---|---|
| **CLI** | Un tunnel direct et large : il peut donner accès à tout un service. | Claude relié à GitHub, à Vercel, ou à tout un espace cloud. |
| **MCP** | Un tunnel par lequel Claude pilote une application. | Claude qui pilote un logiciel. |
| **API** | Un tunnel étroit : on n'ouvre que les fonctions choisies, avec une clé. | Afficher une carte Google Maps sur un site. |

## Se connecter « avec Google » : est-ce risqué ? (question posée)

Non. Le bouton « Continuer avec Google » est une **signature numérique**. Le service ne reçoit
que votre nom et votre adresse email, comme si vous aviez rempli le formulaire à la main.

- Si une application veut un accès plus large (votre Drive, par exemple), une fenêtre vous dit
  précisément à quoi elle aura accès. Vous pouvez refuser.
- Avantage : dans votre compte Google, vous voyez la liste de tous les services où vous êtes
  connecté. Avec des identifiants et mots de passe séparés, impossible de s'en souvenir.
