# Terraform CI

This is reusable Github Action used to deploy Terraform code in NomadHomes.

It requires the following variables:

| Name         | Description     | Required |
|--------------|-----------|------------|
| run-lint | Flag to enable terraform linting as part of the action | false |
| run-plan | Flag to enable terraform plan as part of the action | false |
| run-apply | Flag to enable terraform apply as part of the action | false |
| terraform-dir | Directory of terraform files | false |
| terraform-version | Terraform version to use | true |
| terraform-environment | Environment config to use [dev/prod] | true |
| aws-access-key-id | AWS Access Key ID | true |
| aws-secret-access-key | AWS Secret Access Key | true |
| aws-region | AWS Region | true |