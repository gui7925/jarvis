# Skill : recherche-actualites-contextualisees

> Veille intelligente filtrée selon le contexte personnel de l'utilisateur.

## Déclenchement

Cette skill est activée automatiquement quand l'utilisateur :
- Lance la commande `/morning`
- Demande "fais-moi un point sur les actualités"
- Demande "donne-moi les news du jour"
- Demande "qu'est-ce qui se passe dans [son secteur] ?"

## Ce que fait cette skill

1. Lit le contexte de l'utilisateur (CONTEXT.md) pour comprendre son secteur, ses projets, ses objectifs
2. Recherche des actualités récentes en filtrant par pertinence pour ce contexte spécifique
3. Écarte le bruit (news générales sans lien avec l'utilisateur)
4. Présente uniquement ce qui est utile, avec une analyse d'impact

## Format de sortie

```
**Actualités du jour**
- [Titre] : [1 ligne de contexte]
- [Titre] : [1 ligne de contexte]
- [Titre] : [1 ligne de contexte]

**Ce que ça change pour toi**
- [Actualité 1] : [impact direct en 1 ligne]
- [Actualité 2] : [impact direct en 1 ligne]

**Focus recommandé aujourd'hui**
[1 action concrète et prioritaire]
```

## Principe directeur

Pas de bruit. Seulement ce qui concerne vraiment l'utilisateur, vu ses objectifs et projets actuels.
