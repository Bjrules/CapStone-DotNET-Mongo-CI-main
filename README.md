# CapStone-DotNET-Mongo-CI-main
#### Kinddly see the Capstone-DotNET-Mongo-CD-main
ALL TOOLS PROJECT: This is a Production Grade DevSecOps Project 


![alt text](<FLow Diagaram.png>)

- Set up kubernetes (Terraform with ebs-csi-driver, awscli, kubectl, eksctl, helm)
- Setup and configure HashiCorp Vault inside kubernetes using helm to handle Secrets (In this project it was mongodb's connection string)
- Setup Prometheus, Grafana and the exporters(kubeStateMetrics and nodeExporters) using helm

added resource serviceaccount to role in RBAC
 if certificate status remain false till about 15minute kindly delete it and is will automatically create a new one and pissibly set it's status to true
