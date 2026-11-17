# La démo de la séance 1 : un tableau de bord de reporting, pas à pas

En fin de séance, le formateur a construit en direct, en moins d'une demi-heure, un tableau de
bord de reporting pour un site de vente en ligne fictif. Un développeur y aurait passé des
semaines. Voici le déroulé, pour le refaire chez soi.

## Ce qui a été produit

- Le code de la démo, sur GitHub : https://github.com/AB-Arts/Crea.git
  (dépôt du formateur, rendu public après la séance : c'est un exemple à consulter).
- L'application publiée en séance 2 : https://crea2027.vercel.app
- Le Google Sheet rempli par Claude à partir du tableau de bord : le lien se trouve dans le PDF
  récapitulatif de la séance 1, page « La démonstration, pas à pas ».

## Les étapes

1. **Créer un dépôt privé sur GitHub** et copier son lien en `.git` (voir `05-github.md`).
2. **Créer un dossier vide** sur son ordinateur : ce sera le dossier de travail.
3. **Ouvrir Claude Desktop, mode Code**, créer une conversation et choisir ce dossier sous la
   zone de saisie.
4. **Décrire ce qu'on veut**, à l'écrit ou à la voix, et coller le lien du dépôt. La demande du
   formateur, en substance :

   > Je veux mettre en place une skill qui fait du reporting sur un site de vente en ligne.
   > Pour l'instant, ne te connecte à aucune base de données : mets en place l'interface avec
   > des données fictives. Un site qui vend des vêtements, environ 500 000 € de chiffre
   > d'affaires annuel, une marge d'environ 25 %. Invente des charges pour avoir un tableau de
   > bord hebdomadaire complet. Voici le dépôt où stocker le code, pour en faire une skill
   > ensuite : [lien du dépôt]

5. **Laisser Claude travailler.** Il écrit les fichiers dans le dossier. L'aperçu apparaît à
   droite (l'artefact) : vue d'ensemble, rentabilité, ventes, acquisition, clients, avec un
   mode clair et un mode sombre.
6. **Enregistrer la première version** : « commit la skill sur le Git ». Sur GitHub, le dépôt
   affiche **1 commit**.
7. **Demander une modification** : « ajoute un onglet avec des graphiques en camembert, pour
   voir les ventes par catégorie et par pays. Quand tu as fini, commit. » Le dépôt affiche
   **2 commits**. En cliquant sur le dernier, on voit en vert tout ce qui a été ajouté.
8. **Appliquer une charte graphique** : le formateur a demandé d'utiliser sa skill de charte et
   de refaire le design du tableau de bord, puis un nouveau commit. Sans charte, Claude invente
   un design par défaut.
9. **Revenir en arrière si besoin** : copier le numéro d'un commit et dire « reviens à cette
   version ».

## Le Google Sheet

Pour illustrer une question sur les données, le formateur a créé un Google Sheet vide, l'a
partagé par lien, et a demandé à Claude d'y pousser toutes les données fictives du tableau de
bord. On obtient ainsi un modèle de tableur aligné sur le reporting voulu.

Pour la démo, le partage était ouvert à toute personne ayant le lien, pour aller vite. Pour un
vrai projet, on configure un accès sécurisé au lieu d'un lien ouvert.

## Avec de vraies données

La démo tournait sur des données fictives. Pour passer au réel, on peut :

- donner accès à un Google Sheet partagé ;
- déposer des exports (CSV, Excel) dans le dossier de travail, par exemple les journaux de
  ventes et d'achats du logiciel comptable ;
- relier un service par une **clé d'API** (ventes en ligne, publicité, réseaux sociaux). On
  verra comment ranger ces clés en sécurité : voir `07-cles-api-et-donnees.md`.

## Ce qu'il faut retenir

- **Une fois construit, l'outil tourne.** Tant qu'on ne le modifie pas, on n'a plus besoin de
  l'IA, et on ne régénère pas tout à chaque fois.
- **Les données se mettent-elles à jour seules ?** Pas par défaut. Il faut demander une tâche
  planifiée, ou mettre l'outil en ligne (la suite du module).
- **Claude n'a pas les clés de la maison.** Claude développe l'application. C'est
  l'application qui aura les accès, et elle vous appartient. Comme avec un développeur : il
  part, l'application continue de tourner.
- **Chaque demande est une version.** Le château en Lego se construit semaine après semaine.
