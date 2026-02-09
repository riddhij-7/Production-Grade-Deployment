#  Production-Grade CI/CD Pipeline with Jenkins Multibranch & GitOps

##  End-to-End Deployment Flow

```text
Developer
   ↓
Feature Branch (featureA / featureB)
   ↓
Pull Request → Merge to main (GitHub UI)
   ↓
Jenkins Multibranch Pipeline (CI)
   ↓
Build Docker Image + Push to DockerHub
   ↓
Update Image Tag in Git (K8s Manifest Repo)
   ↓
Argo CD Sync (GitOps)
   ↓
AWS EKS Deployment
   ↓
LoadBalancer URL → Live Application
```




