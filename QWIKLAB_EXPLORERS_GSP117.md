# Setting up Jenkins on Kubernetes Engine || [GSP117](https://www.cloudskillsboost.google/focuses/1776?parent=catalog) ||

## # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers](https://youtube.com/@qwiklabexplorers?si=QGN7mY2Sn9iobmuz) 👍😄🤝

---
## ⚠️ **Disclaimer:**
#### This script and guide are provided for educational purposes to help you understand the lab process. Please ensure you understand the steps before using any scripts. Before using the script, I encourage you to open and review it to understand each step.The goal is to help you learn how to complete the labs effectively while following Qwiklabs' terms of service and YouTube's community guidelines.
---

 - ### Copy & Run the Commands in Cloud Shell Terminal :

```
export ZONE=
```
```
gcloud config set compute/zone $ZONE

git clone https://github.com/GoogleCloudPlatform/continuous-deployment-on-kubernetes.git

cd continuous-deployment-on-kubernetes

gcloud container clusters create jenkins-cd \
--num-nodes 2 \
--scopes "https://www.googleapis.com/auth/projecthosting,cloud-platform"

gcloud container clusters get-credentials jenkins-cd

helm repo add jenkins https://charts.jenkins.io

helm repo update

helm upgrade --install -f jenkins/values.yaml myjenkins jenkins/jenkins
```

---

## Congratulations ..!!🎉  You completed the lab shortly..😃💯

## *Well done..!* 👏

## Thank you for visiting.... :) 🗯️

## [Qwiklab_Explorers](https://youtube.com/@qwiklabexplorers?si=QGN7mY2Sn9iobmuz)

## Join to our community [Digital Dominators](https://linktr.ee/digital_dominators)
