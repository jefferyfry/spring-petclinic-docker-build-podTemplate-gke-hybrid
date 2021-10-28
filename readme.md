# PetClinic Docker Build Pod Template Example for GKE On-Prem Hybrid

[![CIS](https://app.soluble.cloud/api/v1/public/badges/e85d1508-6be2-4dec-9374-1dea7f90c88d.svg)](https://app.soluble.cloud/repos/details/github.com/jefferyfry/spring-petclinic-docker-build-podtemplate-gke-hybrid)  [![IaC](https://app.soluble.cloud/api/v1/public/badges/bf5252f7-a612-48d5-a50c-e920d8259b9b.svg)](https://app.soluble.cloud/repos/details/github.com/jefferyfry/spring-petclinic-docker-build-podtemplate-gke-hybrid)  

This is an example of running an existing Jenkins 2 master on a VM with a GKE On-Prem cluster using the [Kubernetes plugin](https://github.com/jenkinsci/kubernetes-plugin). This allows running an agent pod template on the cluster to handle pipeline tasks. See the [podTemplate folder](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gkeonprem/tree/master/podTemplate) and the [Jenkinsfile](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gkeonprem/blob/master/Jenkinsfile) for details. This pipeline runs a maven build, docker build, pushes the image to docker hub and then deploys the petclinic application to a GKE cloud cluster. This demonstrates a hybrid cloud use case and the scenario of deploying to a cloud staging cluster.

![gke-on prem hybrid - jenkins 2 on-prem](https://user-images.githubusercontent.com/6440106/52495340-3cab1300-2b85-11e9-921a-60b935eb50d4.png)



