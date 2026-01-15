# README for 'Add PR Labels' GitHub Action

## Description

<!-- AUTO-DOC-DESCRIPTION:START - Do not remove or modify this section -->

Adds argocd-deploy and app-specific labels to a PR with random colors

<!-- AUTO-DOC-DESCRIPTION:END -->

The GitHub Action 'Add PR Labels' is a utility action used to tag Pull Requests with specific labels required for deployment workflows (like ArgoCD) or app identification. It ensures the necessary labels exist before applying them.

## Features

- **Automatic Label Creation**: Creates labels if they don't exist.
- **Deployment Tagging**: Adds `argocd-deploy` for deployment triggers.
- **App Identification**: Adds `app:<app_name>` for easy filtering.

## Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|                                          INPUT                                           |  TYPE  | REQUIRED | DEFAULT |                                         DESCRIPTION                                          |
|------------------------------------------------------------------------------------------|--------|----------|---------|----------------------------------------------------------------------------------------------|
|            <a name="input_app_name"></a>[app_name](#input_app_name)                      | string |   true   |         |             The name of the application <br>(e.g., krew-test-app-api)                        |
|           <a name="input_pr_number"></a>[pr_number](#input_pr_number)                    | string |   true   |         |                                  The Pull Request number                                     |
|               <a name="input_token"></a>[token](#input_token)                            | string |   true   |         |                                       GitHub Token                                           |

<!-- AUTO-DOC-INPUT:END -->
