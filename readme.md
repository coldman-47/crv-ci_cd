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

### 1. Créer un cluster Minikube

Une fois installé, vous pouvez démarrer Minikube avec la commande suivante :

```bash
minikube start
```

Ensuite créer le déploiement avec la commande suivante:

```bash
kubectl apply -f deployment.yml
```

Créer ensuite le service en éxécutant la commande suivante:

```bash
kubectl apply -f service.yml
```

Accèder au dashbaord de *Minikube* avec la commande suivante:

```bash
minikube dashboard
```

Pour tester l'application, saisir la commande ci-après dans le terminal:

```bash
minikube service crv-cicd