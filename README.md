# Projet de Sécurisation et Correction de Vulnérabilités

Ce projet consiste à améliorer la sécurité du code d'une application WordPress en identifiant et corrigeant les vulnérabilités à l'aide de **SonarQube** et en automatisant l'intégration continue via **GitHub Actions**.

## Objectifs

1. **Identification et correction des vulnérabilités** :
   - Utilisation de **SonarQube** pour analyser le code à la recherche de vulnérabilités de sécurité telles que les redirections ouvertes, les injections SQL, et d'autres pratiques non sécurisées.
   - Correction des vulnérabilités identifiées pour renforcer la sécurité du code.

2. **Automatisation du processus de vérification** :
   - Mise en place d'un système d'intégration continue avec **GitHub Actions** pour exécuter automatiquement les analyses de SonarQube, ainsi que les tests unitaires à chaque push ou pull request sur la branche `master`.
   - Configuration de **SonarCloud** pour recevoir les résultats d'analyse dans un tableau de bord centralisé et suivre l'amélioration continue du code.

## Technologies Utilisées

- **SonarQube / SonarCloud** : Analyse statique de code pour identifier les vulnérabilités et les problèmes de qualité.
- **GitHub Actions** : Automatisation de l'intégration continue, incluant la vérification des vulnérabilités et l'exécution des tests.


## Fonctionnement

1. **SonarQube** est intégré au projet pour analyser le code à chaque modification apportée. Les résultats de l'analyse sont automatiquement envoyés à **SonarCloud**, où les vulnérabilités et les problèmes sont affichés sur le tableau de bord.
2. **GitHub Actions** est configuré pour exécuter un pipeline CI sur chaque `push` ou `pull request` :
   - Vérification du code avec SonarQube.
   - Exécution des tests unitaires via PHPUnit.
   - Si des problèmes de sécurité ou des erreurs sont détectés, ils sont corrigés directement dans le code.

## Résultats

Vous pouvez consulter les résultats des analyses dans le tableau de bord de **SonarCloud** pour voir l'amélioration de la qualité du code au fur et à mesure des modifications.
