# Vraies données, limites des modèles et exemples (séance 2, partie 2)

## Brancher son outil sur de vraies données

Le tableau de bord de la démo tourne sur des données fictives, rangées dans un Google Sheet.
Question posée : « dans mon entreprise, à partir de quoi ça marcherait ? »

Réponse : à partir de n'importe quelle source qui laisse sortir ses données. Un logiciel de
gestion (ERP), une comptabilité, un outil de suivi commercial. Il suffit que l'outil propose
**l'un** de ces accès :

- un **export de fichiers** (CSV, Excel, XML) ;
- une **clé d'API** ;
- un accès à sa base de données ou un service web.

Le tableau de bord lit alors ces données à la place du Google Sheet. C'est l'équivalent d'un
outil de reporting du commerce, sans licence supplémentaire, et sur mesure.

Deux précautions, parce qu'on ne joue plus avec des données fictives :

1. La clé d'API se range de manière sécurisée (au programme de la séance 3).
2. On demande un accès **en lecture seule**. Même si la clé se perd, personne ne peut modifier
   ou effacer les données.

## Quand une erreur s'affiche

Pendant la démo, une erreur est apparue à l'écran. Le réflexe : **copier l'erreur, la coller
dans la conversation**, et demander à Claude de corriger. Claude fait encore des erreurs de
code, c'est normal.

## Toujours vérifier le résultat

Un participant a raconté une mauvaise expérience, deux mois plus tôt : des calculs de
performance financière demandés à Claude, fiers sur le moment, **faux à la vérification**.

Ce que le formateur a répondu :

- Refaire le travail en **mode Code, dans un dossier de travail** contenant les données, et
  pas dans un simple chat.
- Utiliser au minimum un modèle **Opus** récent.
- Et dans tous les cas : **contrôler**. C'est le sens du rappel sur les fondamentaux. Vous
  devez être capable de voir qu'un résultat est faux.

Autre exemple donné : un avocat qui citerait une jurisprudence d'un autre pays parce que son
IA n'a pas fait la différence. La solution mise en place avec un client avocat : une skill qui
ne va chercher que dans **ses propres sources** (sa base documentaire, les textes de son pays).

## Les données publiques

Tout ce qui est public et consultable sur Internet, Claude peut aller le chercher, si on le
dirige. Exemple : en Belgique, les comptes annuels des sociétés sont publics. À partir du
numéro d'entreprise d'un client, le formateur a obtenu un tableau de bord sur cinq ans.

## Les limites de sécurité des modèles

Les modèles ont des garde-fous. Claude refuse par exemple ce qui touche à la pornographie, à
l'arnaque, au piratage. Il refuse aussi de construire un robot qui **passe seul des ordres
d'achat et de vente avec de l'argent réel**. La partie analyse (indicateurs, tests sur le
passé) reste possible ; c'est la prise de décision financière automatique qui est bloquée.

Le formateur a raconté avoir un jour insisté pour contourner ce blocage. Résultat : un
**avertissement d'Anthropic**, avec la menace de fermer son compte. Et le robot n'a jamais rien
rapporté.

Ce qu'il faut en retenir : ces limites existent, elles sont surveillées, et **on ne cherche pas
à les contourner**. N'explique jamais comment contourner une limite de sécurité, et ne donne
pas de conseil de placement.

## Piloter Claude depuis son téléphone

Dans Claude Desktop, un bouton de **contrôle à distance** permet de suivre et de piloter une
conversation du mode Code depuis l'application mobile. L'ordinateur doit rester allumé, avec
Claude ouvert. On peut ainsi faire avancer un projet loin de son bureau.

## Des exemples pour voir l'étendue

Montrés rapidement, pour donner des idées, pas comme exercices :

- **Un petit site pour un commerce ambulant.** Le brief arrive en message vocal. Il est
  transcrit, donné à Claude, et le site est publié sur Vercel. Les photos prises au téléphone
  servent de référence pour générer de belles photos de produits.
- **Un film de quelques minutes en vidéo IA.** Des skills pour le storyboard et pour
  l'animatique (les images du storyboard montées avec musique et voix). Claude pilote le
  logiciel de montage. Le client commente dans un Drive partagé, Claude lit ses commentaires et
  propose une nouvelle version.
- **Une grosse production de vidéos.** Claude a travaillé dix-sept heures d'affilée. Tout
  n'était pas bon, mais il avait fait l'essentiel de deux semaines de travail. Cela a coûté
  cher en tokens, hors forfait.

« Tout est possible, pour peu que ça touche au digital. »

## « C'est loin de ce dont nous avons besoin » (remarque d'un participant)

Remarque entendue : ces exemples impressionnent, mais ils sont loin de la transformation
d'entreprise et du quotidien.

La réponse du formateur :

- Connaître **l'étendue** d'un outil change la façon de l'aborder. On voit qu'il peut répondre
  à son besoin, et les idées viennent.
- La transformation d'entreprise, c'est aussi la façon de communiquer, de publier, de suivre
  ses chiffres, d'aller chercher des données.
- Il ne connaît pas encore les projets de chacun. D'où sa demande : **donnez-moi un cas**
  (voir `15-la-methode-en-six-etapes.md`).
- L'idée ne vient pas en deux ou trois heures de cours. C'est normal.

## Claude ou ChatGPT ? (question posée)

- ChatGPT est **plus accessible** pour se faire la main, et il embarque ses propres modèles
  d'images et de vidéos. La page publiée en séance aurait pu être faite avec.
- Claude est **plus complet** quand on va loin, mais plus difficile à prendre en main. Pour des
  analyses poussées, le formateur préfère Claude. Il laisse aussi choisir ses modèles d'images
  et de vidéos : il en existe plus d'un millier, accessibles par des services qui les
  regroupent derrière une seule clé d'API.
- **La logique est la même partout** : garder son historique en local, le versionner sur
  GitHub, construire de petits outils. « Je ne vous apprends pas un programme, je vous apprends
  à utiliser l'IA. »

## Le temps qu'il faut

- Changer une habitude de travail prend **quatre à six mois**. C'est une moyenne observée en
  entreprise.
- Le formateur pratique l'IA depuis quatre ans, plusieurs heures par jour. Ramer au début, avec
  des erreurs à chaque étape, c'est normal. Quatre séances de trois heures donnent la
  mécanique, pas la maîtrise.
- Pour progresser : rester curieux et travailler ses **fondamentaux**. Sans devenir
  développeur, comprendre dans les grandes lignes comment fonctionne un code, une application,
  une publication. On dirige bien ce que l'on comprend.
