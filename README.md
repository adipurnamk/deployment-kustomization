# deployment-kustomization

// Short description:
This repository deploys a base Kustomize manifest maintained in a separate repository.

// Detailed tutorial:
## Overview
This repository leverages Kustomize to consume a base manifest hosted elsewhere, streamlining deployments to Kubernetes.

## Prerequisites
- kubectl installed and configured.
- Kustomize available (kubectl has built-in Kustomize support from version 1.14).

## Deployment Tutorial
1. Clone the repository:
   ```
   git clone <your-repo-url>
   cd deployment-kustomization
   ```
2. Deploy the configuration using kubectl:
   ```
   
   kubectl apply -k .
   ```
3. Verify the deployment:
   ```
   kubectl get all -l app=<your-app-label>
   ```

## Customization
Modify overlay configurations as needed to adjust deployment specifics. Ensure the base repository remains accessible.
