# La mémoire et le saucissonnage (séance 1)

## Le problème : la mémoire des modèles s'érode

Tous les modèles ont une mémoire et un historique. C'est un argument commercial : « le modèle
sait qui vous êtes et comment vous travaillez ».

En pratique, un modèle ne garde pas deux ans de données intactes. Situation classique :

1. Vous expliquez quelque chose au modèle. Il se trompe, vous corrigez, il applique enfin bien.
2. Deux semaines plus tard, vous refaites le test. Il refait les mêmes erreurs.

Pourquoi ? Entre-temps, vous avez fait autre chose. Vous avez rempli sa mémoire avec d'autres
informations, devenues plus importantes que la première. **L'historique s'érode avec le temps.**

## La solution : une mémoire à soi

La première chose à faire quand on prototype : créer un **historique qui ne se détériore
pas**. Concrètement, des fichiers (souvent des fichiers `.md`, du simple texte) rangés dans un
dossier du projet, puis sur GitHub.

Cette mécanique n'est pas propre à Claude. Elle fonctionne avec ChatGPT, Gemini, Google AI
Studio ou n'importe quelle interface.

## Le saucissonnage

C'est le nom que le formateur donne à sa méthode.

Imaginez un gros projet : c'est le **saucisson**. On ne le donne pas entier au modèle. On le
**coupe en tranches**, et on travaille une tranche à la fois.

L'exemple du cours : un outil de **reporting hebdomadaire** pour un site de vente en ligne
(produits vendus, statistiques, parcours des clients, export en PDF ou en Excel).

On ne dit pas « fais-moi une application de reporting ». On découpe :

- **Tranche 1 · le design.** À quoi ressemble l'écran final.
- **Tranche 2 · le calcul.** La méthode de calcul de la rentabilité, des ventes, du parcours
  client.
- Puis on **assemble** les tranches en un outil.

Avant tout, on s'assure que le modèle a **compris exactement** ce qu'on lui demande. Les
versions récentes de Claude posent d'elles-mêmes des questions quand il leur manque une
information (quel site, quelle plateforme, quelles données). On peut répondre au fil de l'eau,
ou donner ces informations dès le départ.

## Le handoff

Un **handoff** est l'export du résultat d'une tranche, rangé dans le dossier du projet. Pour
un design, c'est un dossier qui contient la page en HTML, la demande d'origine, et un fichier
qui explique ce que c'est et ce que ça doit faire.

L'idée clé :

- **Créer** le handoff coûte des tokens. On utilise un modèle puissant, jusqu'à être satisfait.
- **Relire** le handoff ne coûte presque rien. Un modèle léger suffit.

## Pourquoi cette méthode

1. **C'est économique.** Les modèles puissants pensent une fois. Les modèles légers exécutent
   ensuite. Rouvrir un chat et lui dire « relis les fichiers du dossier » coûte moins que tout
   réexpliquer.
2. **Ça ne s'oublie pas.** Le projet a sa propre mémoire, hors du modèle.
3. **On n'est pas prisonnier d'un fournisseur.** Si demain Claude triple ses prix et qu'un
   autre modèle coûte moins cher, on branche l'autre modèle sur le même dépôt et il reprend le
   travail.
4. **Ça n'invente pas.** Un outil écrit en code fait toujours la même chose. Le modèle léger
   applique ce qui a été pensé par un modèle plus intelligent.

## L'image de Google Maps

Appeler Google Maps depuis une application coûte très peu, parce que Google Maps est **déjà
développé**. Si vous deviez redévelopper Google Maps à chaque demande, cela coûterait une
fortune.

Sans saucissonnage, c'est ce que vous faites : vous demandez au modèle de tout réinventer à
chaque fois. Avec vos tranches rangées en code, l'outil existe déjà. Il suffit de l'appeler.

Précision donnée en réponse à une question : le saucissonnage ne change pas le prix d'un
service externe comme Google Maps. Ce prix reste le même. Ce qui baisse, c'est le coût des
tokens du modèle.

## Le château en Lego

On construit dans le temps, brique après brique. Chaque semaine, on peut ajouter une
fonctionnalité, en corriger une autre, et garder l'historique complet de ce qui a été fait. Le
château peut devenir immense.

## Un exemple poussé (pour l'idée)

Pour une marque qui publie toujours le même type de vidéo courte : une skill de design (la
typographie, les écrans), une skill de montage, une skill de publication. Quelqu'un filme sur
le terrain, les vidéos arrivent dans un album partagé, l'outil les monte selon la charte et les
dépose en brouillon. Il ne reste qu'à valider. C'est un exemple pour montrer l'empilement des
tranches, pas un exercice du module.
