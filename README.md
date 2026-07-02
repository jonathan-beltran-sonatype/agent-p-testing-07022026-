# How to Use This Template

This repository provides a template for setting up your application deployment using Flux and Kubernetes. The substitution of the necessary values is now automated through a GitHub Actions workflow.

## Step-by-Step Guide

1. **Clone the Repository**: Begin by cloning this template repository to your local environment.

2. **Trigger the Setup Workflow**:
   - Go to the "Actions" tab in your GitHub repository.
   - Select the "Initial Setup" workflow from the list.
   - Click on "Run workflow".
   - Fill in the following inputs:
     - **Product Name**: The name of your product (e.g., `bnr-helloworld-ws`).
     - **Team Name**: The name of your team (e.g., `build-release`).
     - **Image Path**: The path to your container image (e.g., `bnr/helloworld-ws`).
     - **Image Tag**: The tag you wish to deploy (e.g., `0.6.0-202405312041`).
     - **Container Port**: The port you wish to expose (e.g., `8080`).

3. **Review the Pull Request**:
   - After the workflow completes, a PR will be automatically created with the substituted values.
   - Review the PR to ensure everything looks correct.
   - Merge the PR into the main branch.

4. **Deploy Your Application**:
   - Once the PR is merged, your deployment configuration is ready.
   - You can see the status of the deployment by using the flux and kubectl binaries like: `flux get all -n <team_name>-staging-<product_name>` and also `kubectl get all -n <team_name>-staging-<product_name>` 

## Additional Information
   - Ensure you have the proper access to the EKS-Cloudy cluster.
   - Ensure you have the kubectl and flux binaries installed on your laptop.
