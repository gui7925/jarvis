# Commande /update

Objectif : Mettre à jour les fichiers de contexte avec les derniers changements.

## Instructions pour Claude

1. Lis les fichiers actuels :
   - `CLAUDE.md`
   - `context/CONTEXT.md`
   - `context/HISTORY.md`

2. Analyse la conversation récente pour identifier les changements importants :
   - Nouveau projet lancé ou terminé
   - Changement de situation professionnelle ou personnelle
   - Nouvel objectif défini ou objectif atteint
   - Décision stratégique prise
   - Nouvelle information importante sur le contexte

3. Propose à l'utilisateur une liste des mises à jour détectées avant d'écrire quoi que ce soit :
   "Voici ce que je propose de mettre à jour : [liste]. Je confirme avant d'écrire ?"

4. Une fois confirmé, mets à jour les fichiers concernés et ajoute une entrée dans `context/HISTORY.md` avec la date du jour.

## Format d'entrée dans HISTORY.md

```
## [AAAA-MM-JJ]

### [Titre court décrivant la session ou le changement]
- [Changement 1]
- [Changement 2]
- [Changement 3]
```

## Règles

- Ne modifie que ce qui a changé, ne réécris pas tout
- Reste synthétique dans HISTORY.md, une entrée ne doit pas dépasser 10 lignes
- Si rien n'a changé d'important, dis-le clairement plutôt que d'écrire une entrée vide
