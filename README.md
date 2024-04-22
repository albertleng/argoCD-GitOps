# argoCD-GitOps

## Description

This project deploys a Node.js application using ArgoCD and Kubernetes. The application is containerized using Docker and hosted on Amazon ECR.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Ensure you have Kubernetes and ArgoCD installed in your environment.
2. Clone this repository.
3. Apply the Kubernetes manifests in the following order:
   - Deployment.yaml
   - Service.yaml
   - Ingress.yaml

## Usage

The application is accessible at `albert-argocd-gitops.sctp-sandbox.com`. It runs on port 80 and responds to HTTP requests at the root path (`/`).

## Kubernetes Resources

- Deployment: `albert-hello-node` - This deploys the application, ensuring there is always one replica running.
- Service: `albert-hello-node` - This exposes the application on port 80.
- Ingress: `albert-hello-node` - This routes external HTTP traffic to the service.

## Contributing

If you want others to contribute to your project, provide instructions on how to do so. You might also want to include information about your code of conduct.

## License

Include information about your project's license here. If you're not sure what to include, check out [Choose a License](https://choosealicense.com/), a site provided by GitHub that can help you select the right license for your project.

## Contact

If you want to provide contact information for users who have questions or want to get in touch, include it in this section.