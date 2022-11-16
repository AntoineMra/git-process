# Git Process

## Branch Naming Convention

Chaque branche correspond à un objectif précis. Le naming correspond à la structure suivante : `prefix/subject`.

Les prefix sont définit selon la [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/) et le sujet se réfère au context de développement, généralement lié à une User Story du projet.

```bash
# Ajout de la fonctionnalité lié à l'US 24 
feat/24

# Correction d'urgence lié au déploiement
hotfix/deploy

# Correction sur la fonctionnalité lié à l'US 24 
fix/24
```


## Branch Protection

Le code de la branche `main` doit passer les tests, build proprement et être toujours à jour. La branche `main` a besoin de ces qualités pour que les branches de features créées par l'équipe partent d'une version fonctionnelle et propre du code.

- Pour garder la branche `main` la plus propre possible, elle est protégée de toute modifications direct.
- Pour ajouter des modification sur la branche `main`, il faut proposer à l'équipe une proposition de fusion de son travail avec la branche `main`. Cela permet d'échanger entre les membres de l'équipe et obtenir la meilleur version du code possible.

## PR

Les Pull Request représente une proposition de fusion entre la branche `main` et une branche de travail qui est poussé sur le repository.
Pour pouvoir procéder à la fusion, les Pull Request doivent être approuvées par au moins un autre membre de l'équipe avant d'être fusionnées.
Les Reviewers mettent en avant tous les points qui peuvent poser questions (Refactoring, Incohérence, Superflux)
Si la PR est proposé en mode 'Brouillon' ( Elle contient certains éléments pas encore prêt à être fusionnés ) alors le nom de la PR sera préfixé par **Draft:**

## Commits

**Commit fréquent + commit compréhensible** 
Essayez de ne pas oublier de push tous les commits en attente vers le dépôt distant à la fin de chaque journée afin que tout le travail en cours soit sauvegardé.

Le naming correspond à la structure suivante : `prefix(subject): message`.
Les prefix sont définit selon la [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/) et le sujet se réfère au context de développement, généralement lié à une User Story du projet.
Tous les commits ont des messages détaillés et utiles pour décrire la fonctionnalité qui a été codée.

## Deleting Branches

Les branches se supprimeront automatiquement après les PR fusionnées dans `main`. Cela permet de garder le repository propre et d'indiquer clairement où se trouve le développement actif.

# How to ...

## Créer une nouvelle branche pour implémenter une fonctionnalité

To Be Written

## Publier une branche sur le repository distant

To Be Written

## Proposer une Pull Request

To Be Written
