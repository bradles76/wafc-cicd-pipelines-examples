# wafc-devops-pipelines-examples
A few examples of using CI/CD pipelines on Azure DevOps and GitHub Actions to deploy to Web App for Containers

The below folders contains the following:

**azure-devops**:
- `azure-pipelines.yml` contains the yaml used to build and push an image to Azure Container Registry and set this image to be used on the App Service side.

**github-actions**:
- `service-pricipal-auth.yml` contains the yaml used to build and push an image to Azure Container Registry and set this image to be used on the App Service side. This uses Service Principal authentication to authenticate with the container registry, for pushing images in the pipeline.
- `user-password-auth.yml` contains the yaml used to build and push an image to Azure Container Registry and set this image to be used on the App Service side. This uses Username and Password based authentication to authenticate with the container registry, for pushing images in the pipeline.

