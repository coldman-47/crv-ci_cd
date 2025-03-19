# Mise en place du CI/CD avec GitHub Actions pour le déploiement sur Minikube

Ce projet met en place un pipeline CI/CD utilisant **GitHub Actions** pour automatiser le processus de déploiement d'une application dans un cluster **Minikube** avec des conteneurs Docker.

## Prérequis

Avant de commencer, vous devez avoir les éléments suivants installés sur votre machine :

- **GitHub Account** et accès à votre repository
- **Minikube** : Pour lancer un cluster Kubernetes localement
- **Kubectl** : Pour interagir avec Kubernetes
- **Docker** : Pour construire et pousser les images Docker
- **GitHub Actions** : Vous devez avoir un workflow GitHub Action configuré

## Étapes d'installation


Une fois installé, vous pouvez démarrer Minikube avec la commande suivante :

```bash
minikube start

