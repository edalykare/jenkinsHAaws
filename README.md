# jenkinsHAaws
Projet Configuration d'une Haute disponibilté de Jenkins à l'aide de service AWS (Terraform + Ansible + Packer)
## Outils
- GitHub: Repo IaC
- Packer: Build Jenkins Controller and agent AMIs
- Ansible: To configure Jenkins controller and agent during the AMI building process
- Terraform: Provision AWS resources
- Python Boto3: Pour recuperer les clés SSH de AWS parameter store

## Les services AWS
- IAM
- EFS
- AWS parameter store
- Autoscaling Group
- Application Load Balancer
