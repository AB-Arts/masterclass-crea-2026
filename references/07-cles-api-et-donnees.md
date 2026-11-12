# Les clés d'API et la protection des données (séance 1)

## Ce qu'est une clé d'API

Une **clé d'API** est une longue suite de caractères fournie par un service (agenda, logiciel
de facturation, générateur d'images). Elle permet à **une application de se connecter à une
autre**, et d'agir sur votre compte.

Celui qui a votre clé peut utiliser le service **à votre place, sur votre compte**.

## La règle absolue

**On ne colle jamais une clé d'API dans un chat d'IA.** Aucun chat, jamais.

Pourquoi :

- Collée dans un chat, la clé se retrouve en clair sur l'ordinateur, lisible par toute
  personne ou tout logiciel malveillant qui y accède.
- Elle peut partir sur les serveurs du fournisseur du chat.

Ce que ça peut coûter :

- Une clé de **facturation** volée : quelqu'un peut émettre des factures à votre nom, en
  changeant le numéro de compte.
- Une clé de **génération d'images ou de vidéos** volée : vous ouvrez votre compte et
  découvrez des milliers d'euros de consommation.

Deuxième réflexe, déjà vu : un dépôt GitHub est **privé**, pour qu'une clé oubliée dedans ne
soit pas lisible par tous.

Il existe des façons correctes de donner une clé à une application. **Elles sont au programme
de la séance 2.** D'ici là : aucune clé dans un chat.

## Claude a-t-il « les clés de la maison » ? (question posée en séance)

Non. Tant qu'on ne donne pas les clés à Claude, Claude n'a pas d'accès. Claude **développe
l'application** ; c'est l'application qui détient les clés, et elle vous appartient. On peut
couper Claude ensuite, l'application continue de fonctionner.

## Les données de l'entreprise (question posée en séance)

Question : où vont les données, et qu'en est-il de la confidentialité ?

Ce qui a été dit :

- Il y a deux façons de travailler : le modèle lit des fichiers **sur l'ordinateur**, ou l'on
  envoie des données **en ligne**. Dans les deux cas, le traitement par le modèle se fait sur
  les serveurs du fournisseur.
- Avec un **abonnement individuel**, on n'a pas les garanties d'un contrat d'entreprise.
- Une entreprise qui utilise l'IA pour de bon prend un **compte entreprise** chez le
  fournisseur et signe un **DPA** : un contrat qui dit quelles données sont envoyées, comment
  elles sont traitées, où elles sont hébergées, et ce que le fournisseur a le droit d'en faire.
- Le **DPO** (*Data Protection Officer*, délégué à la protection des données) est la personne
  qui s'occupe de ce sujet dans l'entreprise.
- Certains fournisseurs permettent de travailler **uniquement sur des serveurs européens**.
  C'est le cas des modèles Google via Google Cloud, que le formateur propose à ses clients en
  tant que partenaire Google.
- Il faut **se renseigner et vérifier le contrat** de chaque outil que l'on utilise, y compris
  la base de données et l'hébergement. Un fournisseur peut aussi refuser certains types de
  données sensibles.

Le formateur travaille pour des clients du secteur pharmaceutique et est audité sur la
protection des données : c'est une des raisons de ses choix d'outils.

Pour le module, les prototypes se construisent avec des **données fictives**.

## CLI, MCP, API : trois façons de connecter Claude (survol)

Un participant a dit en fin de séance qu'il n'était « pas encore au clair » avec ces mots. La
réponse : c'est normal, on y revient. Voici ce qui a été dit, simplement :

| Mot | Ce que c'est, tel que montré | Exemple de la séance |
|---|---|---|
| **CLI** | Une connexion directe entre Claude et un service, autorisée une fois dans le navigateur. | La connexion à GitHub. |
| **MCP** | Une connexion entre Claude et une application, qui permet à Claude de la piloter. | Claude pilote un logiciel de montage vidéo et cale des textes sur une voix. |
| **API** | La porte d'entrée d'un service externe, ouverte par une clé d'API. | Google Maps, un logiciel de facturation, les plateformes publicitaires. |

Avec ces trois types de connexion, des skills et des versions sur GitHub, les possibilités sont
très larges. Le détail vient dans les séances suivantes.

## La sécurité au quotidien (survol)

Le formateur a relié Claude à ses emails : quand une alerte de sécurité arrive pour une des
technologies de ses applications, la mise à jour est faite aussitôt. Les attaquants reçoivent
les mêmes alertes et agissent vite : il faut être équipé pour réagir aussi vite.
