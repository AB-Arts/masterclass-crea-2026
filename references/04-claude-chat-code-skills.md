# Claude : le Chat, le Code, les connecteurs, les plugins et les skills (séance 1)

## Claude Desktop

Le formateur travaille dans **Claude Desktop**, l'application à installer sur l'ordinateur. On
la télécharge depuis le site de Claude (bouton de téléchargement de l'application de bureau).
Ce n'est pas la version dans le navigateur : **les connecteurs se règlent dans l'application**,
pas dans le navigateur.

## Le mode Chat et le mode Code

| | Mode Chat | Mode Code |
|---|---|---|
| Ce que c'est | Une discussion isolée avec Claude. | Une discussion **liée à un dossier** de votre ordinateur. |
| Où va le travail | Dans l'historique de Claude. Rien n'est rangé sur votre ordinateur. | Dans le dossier choisi. Tout ce que Claude produit s'y enregistre. |
| Pour quoi | Réfléchir, poser des questions, cadrer une idée. | Construire : un outil, une skill, un document, une application. |

Dans le mode Code, on choisit le dossier de travail **sous la zone de saisie**, au moment de
créer la conversation. Ce dossier peut être n'importe quel dossier de votre ordinateur, par
exemple celui d'un client.

ChatGPT a aussi ces deux modes, dans sa version payante.

## Ce qui se passe derrière un chat

Un chat n'est pas un modèle. C'est un écran derrière lequel travaille un **réseau d'agents**.
Si votre demande contient une recherche, un texte et une image, le système la découpe, envoie
chaque partie à l'agent spécialisé, vérifie, regroupe, et vous rend un résultat. On appelle cet
ensemble le *harness*.

Claude seul ne génère ni images, ni vidéos, ni son. Pour cela, on lui **connecte des outils
externes**. Il faut voir Claude Code comme un outil qui met en place des processus, et qui
regroupe d'autres outils et d'autres modèles pour accomplir des tâches complexes. C'est vous
qui orchestrez.

## Les connecteurs

Dans les paramètres de l'application, rubrique **Connecteurs**, on relie Claude à ses outils :
messagerie, agenda, Drive, GitHub, etc. Une fois relié, Claude peut y lire et y agir.

## Les plugins

Un **plugin** est une petite application qui se branche à Claude. Elle fait une tâche
répétitive de manière contrôlée : une fois développée, elle fait toujours la même chose, sans
rien inventer.

## Les skills

Une **skill** (une compétence) est un ensemble d'instructions et de code qui dit à Claude
comment faire une tâche précise, toujours de la même façon.

Exemple du formateur : une skill d'offres de prix. Il discute avec Claude, puis il dit « fais
une offre de prix AB-Arts ». Le document sort toujours avec le même design, les mêmes
couleurs, la même police, le même logo, les mêmes blocs au même endroit.

On appelle une skill en tapant **/** dans la zone de saisie, puis son nom.

Autre exemple montré : une skill qui produit des diplômes de karaté.

## Plugin ou skill : la différence (question posée en séance)

- Un **plugin** est une mini-application **branchée à Claude**. Elle est faite pour dialoguer
  avec Claude.
- Une **skill** fait quelque chose, mais n'est pas branchée comme une mini-application.

La grande différence : une skill peut **devenir une fonctionnalité d'une application** que
vous développez ailleurs. C'est plus difficile avec un plugin, pensé pour Claude seulement.

C'est le chemin du module : **une skill devient un outil, puis une application.** Par exemple,
la skill d'offres de prix pourrait être reliée à un formulaire en ligne : un collègue saisit le
nom du client et une description, et l'offre sort.

Tout ce qui s'automatise, c'est du **code**. Quand vous automatisez quelque chose, des lignes
de code sont écrites quelque part, sur votre ordinateur ou en ligne. Vous n'avez pas à les
écrire ni à les lire. Il faut juste le savoir.

## L'artefact

L'**artefact** est la fenêtre qui s'ouvre **à droite** dans Claude. C'est l'aperçu en direct de
ce que Claude est en train de construire : on voit l'application se dessiner pendant qu'il
travaille.

L'outil construit peut ensuite être utilisé dans Claude, hébergé sur un site, ou tourner
seulement sur votre ordinateur.

## Les tâches planifiées (survol)

Claude peut exécuter une tâche à heure fixe (par exemple un rapport chaque semaine). Avec
l'application de bureau, il faut que l'ordinateur reste allumé et que Claude reste ouvert.
