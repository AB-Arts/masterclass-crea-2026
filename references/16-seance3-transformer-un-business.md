# Séance 3 · Transformer un business, et prototyper devant la personne

Séance du jeudi 19 novembre 2026. La première moitié a répondu à une question du groupe :
quel rapport entre ce que l'on apprend et la « transformation d'un business » ?

Les questions et les témoignages sont repris sans nom. Ne cite jamais un participant.

## Ce n'est pas un logiciel que l'on apprend

Plusieurs participants l'ont dit : la séance 2 allait vite et loin, et ils ne voyaient plus le
lien avec leur métier. La réponse du formateur :

- **Un business, c'est une gestion de problèmes** : finances, production, planning,
  communication, ressources humaines. Un bon business règle ses problèmes vite et bien.
- L'IA et les outils du module servent à **régler ces problèmes beaucoup plus vite**. C'est
  cela, la transformation.
- **Il n'y a pas de marche à suivre.** Avant, on retenait « je clique ici, puis là ». Cette
  mécanique ne vaut plus : l'interface est un simple chat, et l'outil se relie à ce que l'on
  veut. Deux personnes arrivent au même résultat par deux chemins différents. Changer cette
  habitude prend quatre à six mois.

## L'exemple du camion

Une entreprise de chapes perd son camion un lundi. Dix chantiers sont prévus dans la semaine.
Il faut prévenir chaque client, trouver un sous-traitant, refaire le planning, vérifier les
prix. À la main : une nuit blanche pour la personne qui gère le planning.

Avec un outil relié au planning, aux clients, aux emails et aux disponibilités des
sous-traitants, l'IA propose un nouveau planning et prépare les messages en une dizaine de
minutes. La personne relit et décide.

**La leçon** : pour construire cet outil, il faut savoir comment se gère un planning et quels
services existent. Sans les fondamentaux du métier, c'est l'IA qui t'emmène où elle veut.

## Trois attitudes

- **Partir du besoin des gens.** D'abord écouter ce qui leur prend du temps dans la semaine.
  Ensuite seulement, parler de ce que l'IA sait faire. La liste de ces problèmes est la liste
  des premiers prototypes.
- **Être généraliste.** Avoir une vue d'ensemble, savoir comment les choses fonctionnent sans
  être expert de chacune. Et rester expert du résultat que l'on livre.
- **Être curieux.** Avant d'ouvrir Claude, se demander : « comment ferais-je cela avec des
  humains ? ». La réponse donne le découpage du projet.

## L'artisan et son apprenti

Un artisan a du mal à confier son travail. L'IA est un apprenti qui fait ce qu'on lui montre,
en quelques secondes. C'est déroutant : « à quoi je sers, maintenant ? ». Ce qui se facturait
au temps passé perd de sa valeur. Selon le formateur, la valeur se déplace vers le pilotage de
l'outil, la connaissance du métier et la créativité.

Si une tâche de deux jours tombe à dix secondes, la personne qui la faisait se demande ce
qu'elle va faire : cela se prépare.

## Prototyper devant la personne, en cinq temps

Le cas : un collègue recopie chaque semaine des données à la main.

1. **Écouter** : il explique son besoin. On enregistre l'audio, **avec son accord**.
2. **Écrire** : un outil de transcription en fait un texte. Le formateur utilise NotebookLM.
   On garde tout ce qui a été dit, pas une minute de notes.
3. **Construire** : le texte va dans Claude, qui construit une interface.
4. **Corriger** : la personne la voit et réagit (« ce bouton, non »). On ajuste aussitôt.
5. **Remettre** : le lien du dépôt GitHub part au service informatique, qui peut reprendre.

Le service informatique peut fournir **une skill** qui décrit ses règles. Le prototype les
respecte alors dès le départ.

Même idée pour un appel d'offres : au lieu d'un dossier et d'images, on peut arriver avec un
prototype qui fonctionne. Cela prend autant de temps qu'une présentation.

## Des exemples donnés pour montrer l'échelle

Ce que le formateur a dit avoir construit le jour même :

- une vente à la demande pour une boutique de vêtements personnalisés (page de vente,
  catalogue, plaquette) : le vêtement n'est produit qu'une fois vendu ;
- un bouton de signalement sur ses sites : une capture d'écran crée un ticket sur GitHub,
  Claude lit le ticket, corrige et republie ;
- une skill qui produit un PDF de diplômes à partir d'une liste de noms et de grades ;
- une pièce de rechange : Claude pilote un logiciel de dessin 3D gratuit, dessine la pièce
  cassée et l'envoie à une imprimante 3D.

Il a aussi montré un tableau de bord personnel sur un portefeuille **fictif**, sans résultat.
Ne donne aucun conseil de placement.

## Ce qui reste difficile, ce qui garde sa valeur

- Fabriquer ne suffit pas. Il faut encore **faire connaître et vendre**, et c'est ce qui coûte
  le plus. Ce qui sort aujourd'hui peut être copié demain.
- Le goût, l'expérience, la façon dont un client lit une page gardent leur valeur. Un site
  peut être beau et contenir trop de choses : l'IA aide, mais ce jugement s'apprend.
- « Ce qui a de la valeur prend du temps. » Il faut laisser à son cerveau le temps d'apprendre.

## Les questions du groupe

**Comment facturer, si tout va plus vite ?**
C'est le point le plus difficile, a reconnu le formateur. Les clients ne savent pas encore ce
qui est possible. On vend moins du temps, davantage un résultat et un suivi.

**Mon logiciel de gestion peut-il se relier à Claude ?**
S'il propose une API, oui. Exemple cité : Odoo, où l'on crée un utilisateur doté d'une clé
d'API. Claude travaille alors comme un utilisateur du logiciel.

**Et la comptabilité ?**
Dans l'exemple belge du formateur, les factures électroniques arrivent dans le logiciel,
Claude les classe et prépare les écritures, un comptable valide et envoie. Il a précisé ne pas
connaître les règles suisses.

**Que vont devenir les métiers ?**
C'est un avis du formateur, donné comme tel : des tâches disparaissent, des entreprises
reprennent en interne ce qu'elles sous-traitaient, et de petites structures peuvent s'offrir
des outils qui étaient hors de prix. Ne présente pas cela comme une certitude.

**Que conseiller à nos enfants ?**
La créativité, les mathématiques, et comprendre comment les choses fonctionnent sans tout
savoir fabriquer. La sécurité informatique est citée comme un métier d'avenir.

**Peut-on laisser Claude piloter son ordinateur ?**
Le formateur le fait sur une machine réservée à la production, sans données sensibles, avec
des sauvegardes séparées. En entreprise, c'est le service informatique qui décide de ce que
l'IA peut toucher.

**Quel outil pour transcrire une réunion ?**
Un enregistrement audio, puis NotebookLM ou Google AI Studio. Dans tous les cas, l'accord des
personnes enregistrées.
