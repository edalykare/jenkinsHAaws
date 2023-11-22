# jenkinsHAaws
Projet Configuration d'une Haute disponibilté de Jenkins à l'aide de service AWS (Terraform + Ansible + Packer)
## Outils
- GitHub: Repo IaC
- Packer: Build Jenkins Controller and agent AMIs
- Ansible: To configure Jenkins controller and agent during the AMI building process
- Terraform: Provision AWS resources
- Python Boto3: Pour recuperer les clés SSH de AWS parameter store

## Les services AWS
- IAM : to create IAM Role/Instance Profile for Jenkins controller and agent nodes
- EFS : sauvegarder les données jenkins
- AWS parameter store : store SSH provate and public keys
- Autoscaling Group : To deploy the jenkins controller
- Application Load Balancer : To have a static DNS endpoint for the Jenkins controller instance running in the autoscaling group.
