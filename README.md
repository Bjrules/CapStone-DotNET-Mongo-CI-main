# CapStone-DotNET-Mongo-CI-main
#### Kindly see the Capstone-DotNET-Mongo-CD-main
ALL TOOLS PROJECT: This is a Production Grade DevSecOps Project with full Automation

1. See project image below
2. See jenkinsfiles in both the CapStone-DotNET-Mongo-CI-main and the Capstone-DotNET-Mongo-CD-main
3. Refer to the project setup files

![alt text](<FLow Diagaram.png>)
- [x] create Two Instances (1) for EKS and Config and setup (2) Jenkins for CICD 
- Set up kubernetes (Terraform with ebs-csi-driver, awscli, kubectl, eksctl, helm)
- Deploy StorageClass sc.yaml 
- Setup and configure HashiCorp Vault inside kubernetes using helm to handle Secrets (In this project it was mongodb's connection string)
- Setup Prometheus, Grafana and the exporters(kubeStateMetrics and nodeExporters) using helm
- Setup and Configure Sonarqube with PostgreSQl using helm 
- install mongodb.

Create jenkins on another EC2 to perform CI and CD in the Capstone-DotNET-Mongo-CD-main repo
create webhook to trigger build for the CI job and for the CD job since the CI updates the CD repo

added resource serviceaccount to role in RBAC
 if certificate status remain false till about 15minute kindly delete it and is will automatically create a new one and pissibly set it's status to true
