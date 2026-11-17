# Les questions du groupe et le dépannage (séance 1)

Les questions sont reprises sans nom. Ne cite jamais un participant.

## Questions de fond

**Quelle différence entre un plugin et une skill ?**
Un plugin est une mini-application branchée à Claude. Une skill fait une tâche sans être
branchée comme une mini-application, et peut devenir une fonctionnalité d'une application
développée ailleurs. Voir `04-claude-chat-code-skills.md`.

**C'est Claude qui structure le handoff, ou c'est moi ?**
C'est Claude. Le dossier contient la demande d'origine, un fichier d'explication et les
éléments produits. Voir `02-memoire-et-saucissonnage.md`.

**Est-ce la même chose que la méthode d'amélioration des prompts vue dans un autre module ?**
Non. Cette méthode sert à affiner un prompt. Ici, on range des résultats dans des fichiers pour
construire un outil. Et selon le formateur, on a de moins en moins besoin de peaufiner ses
prompts : il parle à Claude comme à un employé.

**Le saucissonnage réduit-il le coût d'une API externe comme Google Maps ?**
Non, ce prix reste le même. Ce qui baisse, c'est le coût des tokens du modèle.

**Si je reviens demain sur mon outil, Claude doit-il tout régénérer ?**
Non. C'est fait, ça tourne, c'est rangé sur GitHub. Tant qu'on ne modifie rien, on n'a plus
besoin de l'IA.

**Les données se mettent-elles à jour toutes seules quand mon tableur change ?**
Pas par défaut. Il faut demander une tâche planifiée, ou mettre l'outil en ligne.

**Faut-il encore un outil d'analyse ou de tableaux de bord séparé ?**
Pour ce type de reporting, le formateur fait tout dans son outil construit avec Claude, relié
aux données par leurs connexions.

**Des entreprises ont-elles construit leur propre CRM avec l'IA ?**
Oui, une petite entreprise peut aujourd'hui développer assez vite un outil sur mesure. Les très
grandes entreprises changent plus lentement, à cause de leur inertie.

**Qu'est-ce qu'on pourrait construire de simple pour s'entraîner ?**
Tout ce qui vous sert au quotidien : un rappel pour le sport, un outil pour préparer des
vacances, un outil de planification pour votre métier. « Il n'y a plus de limite. »

**Va-t-on pratiquer sur nos ordinateurs à la prochaine séance ?**
Oui.

## Questions pratiques

**Faut-il télécharger GitHub ?**
Non. On crée un compte sur github.com et on travaille en ligne. Attention aux sites qui
proposent des téléchargements douteux.

**Quel abonnement pour suivre le module ?**
Le formateur montre tout dans Claude. Avec une formule à 20 par mois, on est vite bloqué. Le
conseil du groupe : la formule Max pendant un mois. Voir `03-modeles-tokens-abonnements.md`.

**Je suis sur ChatGPT, est-ce que ça suffit ?**
La logique est la même et ChatGPT a aussi une connexion GitHub. Mais le formateur ne peut pas
montrer chaque étape dans toutes les interfaces, et la démo de la séance 1 aurait déjà dépassé
ce que permet une formule à 20 par mois.

**Combien de mémoire vive faut-il ?**
32 Go suffisent pour du texte, de la gestion de projet et des PDF. Beaucoup plus pour l'image
et la vidéo.

**Va-t-on recevoir un résumé ?**
Oui : un PDF récapitulatif après chaque séance, diffusé par CREA. Et à la fin des quatre
séances, cette skill, qui contient l'ensemble du module.

## Dépannage

**GitHub affiche « Too many requests » à la création du compte.**
Pistes données en séance : fermer le navigateur et recommencer ; essayer un autre navigateur
(Chrome plutôt qu'Edge) ; vérifier qu'aucun VPN n'est actif ; essayer avec une adresse
personnelle, car une adresse professionnelle peut être bloquée par son domaine ; essayer depuis
un autre ordinateur.

**Le bouton « Continuer avec Google » ouvre le compte de quelqu'un d'autre.**
Le navigateur est connecté à un autre compte Google. Se déconnecter, ou utiliser une fenêtre de
navigation privée, puis recommencer.

**Claude n'arrive pas à se connecter à GitHub.**
Vérifier dans l'ordre :
1. Être connecté à son compte GitHub **dans le navigateur par défaut**.
2. Travailler dans l'**application Claude Desktop**, pas dans le navigateur.
3. Demander « connecte-toi à GitHub en CLI », puis **autoriser** dans la page qui s'ouvre.
4. Sinon : Paramètres, Connecteurs, chercher GitHub, se connecter.
5. Si une fenêtre s'est ouverte au mauvais endroit, la fermer et relancer la demande.

**Claude propose d'installer des outils GitHub.**
C'est normal : accepter, et choisir la connexion CLI.

**L'installation ou la connexion tourne depuis plusieurs minutes.**
Ce n'est pas normal. L'ordinateur manque peut-être de mémoire vive. Fermer les autres
applications, relancer Claude, réessayer.

**Je ne vois pas l'écran du formateur dans Zoom.**
Zoom affiche parfois un autre partage : choisir le bon onglet d'écran en haut de la fenêtre.

**Je ne sais plus dans quel ordre faire les choses (séance 2).**
Voir `15-la-methode-en-six-etapes.md` : dossier, dépôt privé, lien collé dans la conversation,
construire, commit, puis Vercel.

**Je n'arrive pas à relier Claude à Vercel (séance 2).**
Voir `13-vercel-mettre-en-ligne.md`. Vérifier qu'on est en mode Code, accepter l'installation
de Node.js, valider dans le navigateur avec le code reçu par email.

**Toujours bloqué ?**
Noter le blocage dans « Questions pour Anthony » du fichier de suivi, et le montrer en partage
d'écran à la prochaine séance. Ou écrire à info@ab-arts.be.
