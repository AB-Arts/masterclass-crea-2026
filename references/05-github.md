# GitHub (séance 1)

## À quoi ça sert

**GitHub** (github.com) est un service en ligne, propriété de Microsoft, qui **garde du code et
toutes ses versions**. C'est l'outil passe-partout : presque toutes les interfaces d'IA
proposent une connexion GitHub, parce qu'aucun modèle ne sait garder des versions comme lui.

Un compte est **gratuit**, et il le restera à votre niveau. Cela devient payant quand on
travaille à plusieurs de manière intensive ou qu'on utilise beaucoup de puissance de calcul.

## Le tiroir et les enveloppes

- Vous faites un dessin. Vous le mettez dans une **enveloppe numéro 1**, dans un tiroir.
- Vous ajoutez une oreille au personnage : **enveloppe 2**, dans le même tiroir.
- Vous ajoutez un nœud papillon : **enveloppe 3**.

À tout moment, vous pouvez rouvrir le tiroir et reprendre n'importe quelle enveloppe.

| L'image | Le mot | Ce que c'est |
|---|---|---|
| Le tiroir | Le **dépôt** (en anglais *repository*, souvent « repo ») | Le dossier du projet sur GitHub. « Un super dossier », avec toutes ses versions. |
| Une enveloppe numérotée | Un **commit** | Une version enregistrée, avec la liste de ce qui a changé. |

Sur votre ordinateur, vous n'avez **que la dernière version** : Claude modifie les fichiers sur
place. C'est GitHub qui garde toutes les précédentes. Le dépôt du site du formateur compte 249
commits, celui de ses skills plus de 200.

## Travailler à plusieurs : les branches

Plusieurs personnes peuvent proposer des modifications sur le même projet. Chacune travaille
sur une **branche**. Une personne relit, et **valide ou refuse** chaque proposition. Ce qui est
validé rejoint la version principale. Ce qui est refusé n'y entre pas. Cette validation peut
aussi être confiée à une IA, selon des règles écrites à l'avance.

## Revenir en arrière (question posée en séance)

« J'ai fait les versions 1 à 7, et la 3 n'était pas une bonne idée. Puis-je repartir de la 2
en gardant les suivantes ? » Oui. Claude relit les versions, voit les différences, garde le
reste et réadapte seulement ce qu'il faut, dans une nouvelle version.

Pour revenir à une version précise : copier le numéro du commit et dire à Claude « reviens à
cette version ».

## Créer son compte et son premier dépôt

1. Aller sur **github.com** dans le navigateur et créer un compte. **Rien à télécharger** : on
   travaille en ligne.
2. Cliquer sur le **+** en haut à droite, puis **New repository** (nouveau dépôt).
3. Donner un nom (sans espace, par exemple `crea-masterclass-2026`) et une description.
4. Choisir **Private** (privé). C'est le seul réglage à changer.
5. Créer le dépôt. La page affiche un dépôt vide et un **lien qui se termine par `.git`**.
   Copier ce lien : c'est lui qu'on donne à Claude.

Les modèles proposés par GitHub (« start with a template ») ne servent pas ici.

## Toujours privé

Première règle de sécurité du module : **un dépôt est privé par défaut**. Un dépôt public peut
être lu par n'importe qui. Si une clé d'API s'y retrouve par erreur, le monde entier y a accès.
Privé, c'est votre tiroir : vous seul avez la clé.

## Connecter GitHub à Claude

Deux chemins, au choix :

- **En le demandant** : dans une conversation du mode Code, en étant déjà connecté à GitHub
  dans son navigateur, écrire « connecte-moi à mon GitHub ». Une page s'ouvre dans le
  navigateur pour **autoriser** la connexion. On valide, c'est fait.
- **Par les paramètres** : dans l'application Claude Desktop, Paramètres, **Connecteurs**,
  chercher GitHub, se connecter. La même page d'autorisation s'ouvre.

Si Claude propose plusieurs méthodes, choisir la connexion **CLI** (via l'outil `gh`) : c'est la
plus simple, « ça va tout seul ». L'autre méthode (SSH) est utile aux équipes qui gèrent leurs
propres clés, pas à vous. Claude peut demander d'installer un petit outil GitHub : accepter.

En cas de problème, voir `08-questions-du-groupe-et-depannage.md`.

## GitHub n'est pas Notion (question posée en séance)

Notion sert à gérer des tâches et des projets. GitHub sert à garder du code et ses versions.
Ce sont deux outils différents, que l'on peut relier : un testeur ouvre une tâche dans l'outil
de gestion, Claude la lit, corrige, et enregistre la correction sur GitHub.
