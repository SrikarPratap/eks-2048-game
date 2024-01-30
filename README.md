# AWS EKS Deployment for 2048 Game

Welcome to the AWS EKS project showcasing the deployment of the classic 2048 game. This project leverages key Kubernetes components, including Deployment, Service, Ingress, and Ingress Controller, to provide a scalable and efficient infrastructure for hosting the game.

## Project Overview:

### 2048 Game Deployment:

The project focuses on deploying the popular 2048 game using Kubernetes. A Deployment ensures the game is scalable, maintaining the desired number of replicas to handle varying loads seamlessly. This allows for easy scaling up or down based on demand.

### Service:

A Kubernetes Service is utilized to expose the 2048 game internally, ensuring seamless communication between different components of the application. The Service abstraction provides a stable endpoint for accessing the game, abstracting away the complexities of individual Pod IP addresses.

### Ingress:

To enable external access to the 2048 game, an Ingress resource is employed. Ingress acts as an entry point for external traffic, allowing users to interact with the game over the internet. This provides a clean and flexible way to manage external access and route traffic to the appropriate backend service.

### Ingress Controller:

The Ingress Controller acts as the gateway managing the Ingress resources. It interprets the Ingress rules and ensures that external requests are directed to the correct Services within the EKS cluster. This component enhances the project's scalability, reliability, and routing capabilities.

## Project Structure:

- **/deployment:** Contains Kubernetes Deployment and Ingress configurations responsible for handling external traffic for the 2048 game.
- **/service:** Includes Service configurations for internal communication within the cluster.

## Getting Started:

Follow the steps below to set up and deploy the 2048 game on AWS EKS:

1. Clone the repository: `git clone https://github.com/your-username/eks-2048-game.git`
2. Navigate to the project directory: `cd eks-2048-game`
3. Follow the documentation which consists of commands to install EKS, create fargate profile for the game, to deploy ALB controller and associate oidc connector.
4. Apply Kubernetes configurations: `kubectl apply -f deployments/ -f services/`

Enjoy playing 2048 on your AWS EKS deployment! Feel free to explore and customize the configurations to suit your preferences or integrate additional features.

## Contributions:

Contributions and suggestions are welcome! If you have ideas for improvements or new features, please open an issue or submit a pull request.

Let the gaming begin! 🎮✨