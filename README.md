# Module 5 CREA · Prototypage rapide & MVP avec l'IA · skill de révision et de suivi

Skill Claude pour les participants du **Module 5 « Prototypage rapide & MVP avec l'IA »** du
Cycle Certifiant Transformation Business & IA de **CREA Genève**, donné par **Anthony Beth
(AB-Arts)** en novembre 2026.

Elle fait deux choses :

- **Réviser** : elle répond aux questions sur ce qui a été vu en séance, et seulement cela, au
  niveau débutant du cours.
- **Suivre** : elle tient une check-list par séance, dit quelle est la prochaine étape, et peut
  enregistrer l'avancement dans un fichier `suivi-crea.md` du dossier de travail.

## Installer la skill

Dans Claude Desktop, mode Code, il suffit de demander :

> Installe la skill qui se trouve dans ce dépôt GitHub : https://github.com/AB-Arts/masterclass-crea-2026.git

Ou, à la main, cloner le dépôt dans le dossier des skills de Claude :

```bash
git clone https://github.com/AB-Arts/masterclass-crea-2026.git ~/.claude/skills/ab-arts-masterclass-crea
```

La skill s'appelle ensuite avec `/ab-arts-masterclass-crea`.

## Contenu

```
SKILL.md                                  le comportement de la skill
references/
  00-carte-et-perimetre.md                la carte des sujets, séance par séance
  01-prototype-et-etat-desprit.md         \
  02-memoire-et-saucissonnage.md           |
  03-modeles-tokens-abonnements.md         |
  04-claude-chat-code-skills.md            > séance 1 (12 novembre 2026)
  05-github.md                             |
  06-demo-reporting-pas-a-pas.md           |
  07-cles-api-et-donnees.md                |
  08-questions-du-groupe-et-depannage.md  /
  09-suite-du-module.md                   ce qui arrive dans les séances suivantes
  10-catalogue-academy.md                 les formations AB-Arts, pour aller plus loin
  11-seance2-rappels-et-complements.md    \
  12-api-et-cles-api.md                    |
  13-vercel-mettre-en-ligne.md             > séance 2 (17 novembre 2026)
  14-vraies-donnees-limites-et-exemples.md |
  15-la-methode-en-six-etapes.md          /
  suivi-checklist.md                      la check-list de suivi et le modèle de fichier
```

## Mettre à jour après chaque séance

1. Ajouter les fichiers `references/16-...md` et suivants avec les nouveaux sujets.
2. Compléter `00-carte-et-perimetre.md` : ajouter la séance, sortir les sujets de « pas encore
   vu ».
3. Mettre à jour `09-suite-du-module.md` et ajouter la check-list de la séance dans
   `suivi-checklist.md`.
4. Mettre à jour la description de `SKILL.md` si de nouveaux mots-clés apparaissent.
5. Commit et push.

Aucun nom de participant, aucune donnée personnelle dans ce dépôt.

---

AB-Arts SRL · [ab-arts.be](https://ab-arts.be) · info@ab-arts.be
