# Wavenet - Exemples d'Actions
Dans ce repository, vous pourrez trouver un ensemble de templates d'actions et de pratiques que vous pouvez utiliser dans vos projets.

## Intégration Continue
### Next.js - Yarn 3
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/ci-nextjs.yml

### .Net Framework - MSBuild
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/ci-netframework.yml

### .Net Core - dotnet build - Sonnar
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/ci-netcore.yml

### Front - Gulp - Grunt
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/ci-gulp-grunt.yml

## Déploiement
### .Net - Azure Function - Azure Functions App
Action : https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/cd-azure-functions-app.yml

### .Net Framework - Azure App Service
Action : https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/cd-net-framework.yml

Cette action permet de déployer une application .Net Framework sur un Azure App Service.
Elle contient les tâches qui permettent de faire des actions "legacy" comme la transformation des fichiers de configuration et le remplacement des variables.

Elle contient aussi la génération des fichiers clients avec Gulp / Grunt.

C'est la tâche de base pour les projets "legacy" qui ne sont pas encore migrés vers .Net.

### Docker - Azure Container Registry
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/cd-docker-acr.yml

Cette action permet de générer une image docker depuis un dockerfile et de la publier sur l'Azure Container Registry.

### Docker - GitHub Container Registry
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/cd-docker-ghcr.yml

Cette action permet de générer une image docker depuis un dockerfile et de la publier sur la GitHub Container Registry.

## Release Drafter
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/release-drafter.yml

Configuration: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/release-drafter.yml

Basé sur le travail fourni par cette action : https://github.com/release-drafter/release-drafter, voici un exemple de configuration de Release Drafter que vous pouvez utiliser.

Cet exemple gère des catégories et des tags complémentaires à l'exemple fourni dans la documentation de Release Drafter.

## Utilitaires
### Vérification du tag
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/check-tags.yml

Cette action permet de vérifier si le workflow a bien été lancé par un tag, elle utilise une actions personnalisée présente dans le répository suivant : https://github.com/wavenet-be/wavenet-actions-check-tag

## Transformation des configurations
Action: https://github.com/wavenet-be/wavenet-devops-templates/blob/main/.github/workflows/utility-config-transform.yml

Ce template d'action est un exemple d'utilisation des transformation XML des fichiers Web.Config et du remplacement des variables pour pouvoir effectuer des actions similaires à ce qui était disponible sur Devops avec la gestion des releases.
