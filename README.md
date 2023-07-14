# example1

Information about Localstack and how to setup can be found at [Conciso Confluence](https://conciso.atlassian.net/wiki/spaces/~855124552/pages/3071672390/LocalStack) or [LocalStack Documentation](https://docs.localstack.cloud/) website

Once you setup terraform, pre-commit and aws cli on your system and start LocalStack docker container you can use the commands below

## Initiate terraform 
terraform init
## Format syntax
pre-commit run terraform_fmt --files ./*
## Create this README.md 
pre-commit run terraform_docs --files ./*
pre-commit run terraform_docs_without_aggregate_type_defaults --files ./*
## Validate TF configuration
pre-commit run terraform_validate --files ./*
## Security Check
pre-commit run terraform_checkov --files ./*
## Plan
terraform  plan
## Apply 
terraform apply --auto-approve

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) |  >=1.0.9 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >=4.36.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.59.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_s3_bucket.test-bucket](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |

## Inputs

No inputs.

## Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
