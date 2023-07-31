# wafc-cicd-pipelines-examples

This repository contains examples of using GitHub Actions and Azure DevOps pipelines to build and deploy custom Docker Images to Web Apps for Containers

- `github-actions`:
  - This contains a simple node application that can be build and ran as a custom image
  - `.github/workflows` contains the relevant workflow files
    - `user-password-auth.yml` - This uses Admin Credential (username, password) authentication for Container Registry authentication and a Publish Profile for deployment to App Service
    - `service-principal-auth.yml` - This uses Service Principal authentication for Container Registry, without the `docker/login-action@v1` task authentication and for deployment to App Service
    - `service-principal-auth-v2.yml` - This uses Service Principal authentication for Container Registry, with the `docker/login-action@v1` task authentication and for deployment to App Service