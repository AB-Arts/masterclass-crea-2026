# Séance 3 · Google AI Studio, Vertex AI et les modèles de Google

Vu le jeudi 19 novembre 2026. Les conditions des services évoluent : quand tu donnes un de ces
éléments, précise « tel que dit en séance, à vérifier sur le site de Google ».

## Deux portes vers les mêmes modèles

Google donne accès à ses modèles de deux façons. Les modèles sont les mêmes. Ce qui change,
c'est le contrôle que l'on a sur ses données.

| | Google AI Studio | Vertex AI, dans Google Cloud |
|---|---|---|
| L'image | La porte rapide | La porte de l'entreprise |
| Pour démarrer | Un compte Google et un moyen de paiement. La clé se crée en un clic | Un projet Google Cloud à configurer, en général avec le service informatique |
| Où vont les données | On ne choisit pas la région. Les demandes peuvent être traitées hors d'Europe | On choisit la région des serveurs, par exemple l'Europe |
| Conservation | Peu de réglages | Durée de conservation réglable |
| À utiliser pour | Apprendre et prototyper, avec des données fictives | Un usage professionnel, avec des données réelles |

Adresse : aistudio.google.com. Pour relier Claude à Google Cloud, on passe par l'outil en
ligne de commande de Google Cloud, sur le même principe que pour GitHub et Vercel.

Pour des données de son entreprise, le choix se valide avec le service informatique ou le
délégué à la protection des données. Tu ne donnes pas d'avis juridique.

## Une seule clé pour beaucoup de choses

Avec une clé Google AI Studio, on accède à des modèles de :

- texte ;
- images ;
- vidéo ;
- voix et musique ;
- transcription d'un audio en texte.

Ailleurs, il faut souvent une clé par service.

## Ce que cela coûte

Chaque génération est facturée sur la carte liée au compte. **La vidéo coûte le plus cher.**
En séance, le formateur estimait à quelques euros le coût de ses quelques essais. Conseil :
commencer par des images, limiter la vidéo à un ou deux essais courts en basse résolution.

## Construire dans Google AI Studio

Google AI Studio permet aussi de construire de petites applications. Le formateur le trouve
moins bon que Claude pour développer, mais utile pour s'essayer. Ce qui y est créé est hébergé
chez Google. Il déconseille de mettre tous ses œufs dans le même panier.

## Les droits et les images générées

- Le modèle a refusé de représenter un sportif réel, mais a dessiné un personnage de dessin
  animé connu. **Qu'un modèle génère une image ne donne pas le droit de l'utiliser.**
- Les règles européennes demandent de signaler un contenu produit par une IA. À prendre comme
  habitude dès le prototype.
- Certains modèles de vidéo sont exploités hors d'Europe. Avant d'y envoyer un contenu
  professionnel, vérifier où il part.

## Les connexions MCP pour générer des images

Le formateur a seulement dit que cela existe : on peut relier à Claude un service de
génération d'images et de vidéos, pour illustrer un prototype sans quitter la conversation. Il
a cité son propre studio. La manipulation n'a pas été montrée.
