# Setup — comment utiliser ces skills

Ce repo contient des **Agent Skills Claude** (format `SKILL.md`) extraites de
*The 10x Method* (Hexa). Chaque skill apprend à Claude un framework précis du
livre pour l'appliquer à ta propre startup. Ce guide explique comment les
installer et les déclencher, que tu utilises **Claude Code** (CLI/VS
Code/web) ou **claude.ai**.

## 1. Où copier les skills

Chaque dossier `skills/<nom-de-skill>/` (avec son `SKILL.md` et, pour
certaines, un sous-dossier `references/`) doit être copié dans un dossier
`skills/` reconnu par Claude. Deux portées possibles :

**Option A — Une seule startup / projet (recommandé pour démarrer)**

Copie les skills que tu veux dans le dossier `.claude/skills/` à la racine
du repo de ton projet :

```bash
mkdir -p /chemin/vers/ton-projet/.claude/skills
cp -r skills/idea-categorizer /chemin/vers/ton-projet/.claude/skills/
cp -r skills/mvp-scope-checker /chemin/vers/ton-projet/.claude/skills/
# ... répète pour chaque skill voulue, ou copie tout le dossier :
cp -r skills/* /chemin/vers/ton-projet/.claude/skills/
```

Elles ne seront disponibles que dans les sessions Claude Code ouvertes sur
ce projet.

**Option B — Toutes tes startups / usage perso**

Copie-les dans ton dossier utilisateur global, disponible dans toutes tes
sessions Claude Code :

```bash
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/
```

**Option C — claude.ai (interface web/app)**

Dans les paramètres de ton Projet (ou de ton compte, selon ton plan), va
dans la section **Skills / Capabilities** et importe chaque dossier
`skills/<nom>/` (ou uploade son contenu en zip si l'interface le demande).
Le contenu et le format (`SKILL.md` + `references/`) sont identiques.

## 2. Comment ça se déclenche

Pas besoin de "lancer" une skill manuellement : Claude lit le champ
`description` de chaque `SKILL.md` et déclenche la bonne skill tout seul
quand ta question y correspond.

Exemples de phrases qui déclenchent automatiquement une skill :
- *"J'ai une idée de startup dans la fintech, tu en penses quoi ?"* → `idea-categorizer`
- *"Voici mon plan MVP, est-ce que j'en fais trop ?"* → `mvp-scope-checker`
- *"Aide-moi à écrire la JD pour mon premier ingé"* → `job-description-builder`
- *"Je prépare mon pitch deck pour la levée"* → `pitch-deck-structure-builder`

Tu peux aussi être explicite : *"Utilise la skill scorecard-builder pour
préparer mes entretiens"*.

Si une skill ne se déclenche pas comme attendu, vérifie que :
1. le dossier est bien copié à l'un des emplacements ci-dessus,
2. le nom du dossier correspond au `name:` du frontmatter,
3. tu as ouvert une **nouvelle session** Claude Code après la copie (les
   skills sont chargées au démarrage de la session).

## 3. Dans quel ordre les utiliser

Les skills suivent globalement la progression du livre. Utile si tu
construis une startup de zéro, mais chaque skill fonctionne aussi de façon
indépendante :

| Étape | Skill(s) | Chapitre |
|---|---|---|
| 1. Trouver et valider l'idée | `idea-categorizer`, `idea-validation-roadmap-builder` | Ch.II |
| 2. Choisir son cofondateur | `cofounder-alignment-assessor` | Ch.III |
| 3. Construire le MVP | `mvp-scope-checker`, `milestone-roadmap-builder` | Ch.IV |
| 4. Recruter les premiers talents | `job-description-builder`, `scorecard-builder` | Ch.V |
| 5. Trouver les premiers clients | `design-partner-deck-builder`, `bant-qualifier` | Ch.VI |
| 6. Brand & communication | `brand-foundations-builder`, `brand-voice-finder` | Ch.VII |
| 7. Lever des fonds | `executive-summary-builder`, `pitch-deck-structure-builder`, `data-room-builder` | Ch.VIII |
| 8. ESG dès le début | `esg-checklist` | Ch.IX |

Pour le contexte complet d'un chapitre (résumé, citations, frameworks
annexes non transformés en skill), consulte le fichier correspondant dans
`chapter-readmes/`.

## 4. Mettre à jour ou ajouter des skills

Si tu modifies un `SKILL.md` déjà installé, recopie-le à l'emplacement
choisi à l'étape 1 puis redémarre ta session Claude Code pour que le
changement soit pris en compte. Les nouvelles skills ajoutées à ce repo (cf.
la liste "reste à faire" dans le `README.md`) s'installent de la même
façon.
