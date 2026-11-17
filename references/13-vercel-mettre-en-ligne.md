# Vercel : mettre son prototype en ligne (séance 2, partie 1)

## Pourquoi un outil de plus

Avec GitHub seul, l'application reste sur votre ordinateur. C'est déjà suffisant pour beaucoup
d'usages. Mais pour un site, ou un formulaire à envoyer à des clients, il faut une adresse web.

Il faut donc un **outil de déploiement**. *Déployer*, c'est mettre en ligne. Il en existe
beaucoup. Le formateur propose **Vercel** (vercel.com) : gratuit pour commencer, simple, et
très bien relié à Claude et à GitHub.

Vercel n'est pas une place de marché. C'est un **hébergeur** doté d'un système qui va chercher
le code sur GitHub et le publie.

Le but du module n'est pas de vendre Vercel. Il est de comprendre que Claude se connecte à des
outils, et qu'une application construite en local peut être publiée.

## Créer son compte

1. Aller sur vercel.com et se connecter avec son compte Google.
2. À la question sur le type de projet, choisir **projet personnel** : c'est gratuit.

La différence, telle qu'expliquée en séance : en gratuit, le site est hébergé sur des serveurs
américains. Avec une formule payante, on peut choisir la région des serveurs, par exemple en
Europe. Pour un prototype avec des données fictives, le gratuit convient.

## Relier Claude à Vercel (à faire une seule fois)

Démonstration faite en direct sur l'écran d'une participante.

1. À la création du compte, Vercel propose d'**intégrer son agent** (« Onboard your agent ») et
   donne une ligne à copier.
2. Ouvrir Claude Desktop en **mode Code**, pas en mode Chat, dans un dossier de travail.
3. **Coller cette ligne** et suivre ce que Claude demande.
4. Claude installe ce qu'il lui faut, dont un outil technique nommé **Node.js**. Accepter. S'il
   demande de le faire à la main, répondre : « Installe-le toi-même. »
5. **Valider la connexion** dans le navigateur, puis saisir le code reçu par email. Ces
   sécurités empêchent qu'une application soit publiée depuis votre ordinateur sans vous.
6. Si Claude propose en plus une connexion **MCP**, on peut la passer : la connexion CLI
   suffit.
7. Vérifier : « Est-ce que je peux déployer des applications maintenant ? » Inutile de lancer
   un test.

Règle générale donnée à ce moment : n'hésitez pas à demander à Claude de faire lui-même ce que
vous ne comprenez pas dans ce genre d'installation.

## Publier son application

Le formateur a publié le tableau de bord de la séance 1.

1. **Prévenir Claude.** Il avait construit un outil pour l'ordinateur, pas pour le web :

   > Le dashboard me convient. Je vais le déployer sur un nouveau projet Vercel. Vérifie si le
   > code est prêt pour le déploiement.

   Claude adapte le code. Il utilise une technologie nommée **Next.js**, qui fonctionne très
   bien avec Vercel. Vous n'êtes pas obligé de la nommer.
2. **Refuser que Claude déploie lui-même**, et lui dire : « Non, je le fais moi-même, mais
   commit sur GitHub. » Claude sait déployer, mais il choisirait le nom et les réglages à votre
   place. Le formateur préfère garder la main.
3. Dans Vercel, **créer un nouveau projet**, cliquer sur GitHub pour le relier, puis
   **importer le dépôt**.
4. **Donner un nom** au projet. Ne pas toucher aux autres réglages.
5. Cliquer sur **Déployer**. Vercel prend la dernière version sur GitHub, la compile et la met
   en ligne.
6. L'application reçoit une **adresse en `.vercel.app`**, à partager.

## Ensuite, tout est automatique

Chaque nouveau commit sur GitHub **redéploie le site tout seul**. Dans Vercel, la rubrique des
déploiements montre l'historique.

Démonstration : le formateur a demandé, à la voix, que chaque section devienne une page
séparée avec sa propre adresse, et que le tout soit **responsive** (adapté au téléphone, quelle
que soit la taille de l'écran). Trois minutes plus tard : nouveau commit, nouveau déploiement,
site à jour. Un développeur y aurait passé un ou deux jours, voire plus.

Mots entendus :

- Une **route** : l'adresse d'une page à l'intérieur du site.
- Un ***one pager*** : un site d'une seule page, où les boutons font défiler.
- **Responsive** : qui s'adapte à la taille de l'écran.

## Claude teste comme un humain

Claude clique réellement sur les boutons, à plusieurs tailles d'écran, et corrige ce qui
s'affiche mal. Ces vérifications peuvent être **écrites et gardées** dans le dépôt, puis
rejouées à chaque nouvelle version. Cela évite les **régressions** : qu'une modification
casse, sans qu'on le voie, quelque chose qui marchait.

## Le nom de domaine (question posée)

- Par défaut, l'adresse se termine par `.vercel.app`. C'est fait pour tester.
- On peut y relier **son propre nom de domaine**, dans la rubrique des domaines du projet. Il
  faut alors modifier un réglage (les DNS) chez le fournisseur du nom de domaine.
- On ne peut pas avoir deux sites sur le même nom. On crée un **sous-domaine**, par exemple
  `app.monsite.ch` pour l'application, à côté du site existant.
- Le formateur n'est pas allé plus loin : trop technique pour ce stade.

Dans le projet Vercel, à côté des domaines, se trouvent les **variables d'environnement** :
c'est là qu'iront les secrets et les clés d'API. Voir `12-api-et-cles-api.md`.

## Et les autres solutions ? (questions posées)

- **Un hébergeur suisse comme Infomaniak** : le principe est possible, il propose aussi un
  déploiement depuis GitHub. Le formateur ne l'utilise pas et ne peut pas dire si c'est aussi
  simple. Il n'a pas trouvé de connecteur officiel pour Claude. À demander à l'hébergeur.
- **Netlify** : même mécanique.
- **Lovable et les outils du même type** : ils font toutes ces étapes à votre place, avec
  Claude derrière. C'est plus simple, mais selon l'expérience du formateur les tokens y coûtent
  beaucoup plus cher, et on est vite limité. Faire soi-même avec Claude, GitHub et Vercel
  revient bien moins cher.

## Prototype, pas production

Rappel ferme du formateur. Ici, on **prototype** :

- pas de vraies données, pas de données de clients ;
- pas toutes les sécurités, pas forcément les bons serveurs ;
- on s'arrête à « mon application est en ligne et je peux la montrer ».

Aller plus loin est possible : un vrai nom de domaine, le choix des serveurs, les sécurités.
Mais c'est une autre étape.

## « Et moi, je n'ai pas encore d'application à publier »

Remarque d'un participant, tout à fait normale. Les connexions (GitHub, Vercel) se font une
fois. Ensuite, il faut d'abord construire quelque chose, même tout petit, comme dans
`06-demo-reporting-pas-a-pas.md`, puis le publier en suivant ce fichier.

## Ce que ça change, encore

Le formateur a raconté avoir construit en dix minutes, pour une responsable commerciale, un
outil qui faisait sa saisie d'une semaine. Sa réaction : « J'ai vingt-cinq ans d'expérience, et
tu viens de faire mon travail en dix minutes. » Le message : l'outil ne prend pas le travail,
il libère du temps pour aller plus loin. Et un concurrent qui s'en sert ira beaucoup plus vite
que celui qui ne s'en sert pas.
