# JCasC with Linux & Windows agents in Kubernetes

In this project we want to create a Jenkins in our Kubernetes cluster with JCasC configurations!

first of all, you need a Kubernetes cluster up and running
second of all, we need to pull the [jenkins official helm chart](https://github.com/jenkinsci/helm-charts)

then after pulling it via ```helm pull jenkins/jenkins``` into your computer, we need to change some of its values for our desired configs!

I will list some important values for our Jenkins helm chart!
- Your Jenkins image
- Your admin password
- Resource allocation for Jenkins based on your need and the scale of your application
- Configuration for your desired plugins to install in Jenkins and ``` configuration as code``` is a must in this scenario
- The Jcasc key must be set to True with your needed configurations
- Configuration for auto-reload if you want your configs to reload automatically
  
