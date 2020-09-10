# Setting CI/CD for Data Lake work loads with Terraform, Cloud Build, and GitOps

This tutorial explains how to manage infrastructure as code with Terraform and Cloud Build using the popular GitOps methodology for Data Lake pipelines


## Configuring your **dev** environment

Just for demostration, this step will:

 1. Create Data Flow
    1. Transform source data
    2. Create Big Query Dataset
    3. Create Tables
    4. Write data into Big Query Table

```bash
cd ../environments/dev
terraform init
terraform plan
terraform apply
terraform destroy
```

## Promoting your environment to **production**

Once you have tested and validated your Data Lake in DEV you can pomote to PROD 

```bash
cd ../prod
terraform init
terraform plan
terraform apply
terraform destroy
```
