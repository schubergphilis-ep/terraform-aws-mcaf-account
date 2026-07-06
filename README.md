# terraform-aws-mcaf-account

MCAF terraform module to create an AWS account using Control Tower's Account Factory.

<!--- BEGIN_TF_DOCS --->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.13 |
| mcaf | >= 0.4.2 |

## Providers

| Name | Version |
|------|---------|
| mcaf | >= 0.4.2 |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| account | The name of the account | `string` | n/a | yes |
| email | Email address of the account | `string` | n/a | yes |
| organizational\_unit | Organization unit to create the account in | `string` | n/a | yes |
| sso\_email | The email address of the Control Tower SSO account | `string` | n/a | yes |
| provisioned\_product\_name | A custom name for the provisioned product | `string` | `null` | no |
| sso\_firstname | The first name of the Control Tower SSO account | `string` | `"AWS Control Tower"` | no |
| sso\_lastname | The last name of the Control Tower SSO account | `string` | `"Admin"` | no |

## Outputs

| Name | Description |
|------|-------------|
| id | The AWS account ID |
| name | The AWS account name |

<!--- END_TF_DOCS --->

## License

**Copyright:** Schuberg Philis

```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13 |
| <a name="requirement_mcaf"></a> [mcaf](#requirement\_mcaf) | >= 0.4.2 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_mcaf"></a> [mcaf](#provider\_mcaf) | >= 0.4.2 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [mcaf_aws_account.default](https://registry.terraform.io/providers/schubergphilis/mcaf/latest/docs/resources/aws_account) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_account"></a> [account](#input\_account) | The name of the account | `string` | n/a | yes |
| <a name="input_email"></a> [email](#input\_email) | Email address of the account | `string` | n/a | yes |
| <a name="input_organizational_unit"></a> [organizational\_unit](#input\_organizational\_unit) | Organization unit to create the account in | `string` | n/a | yes |
| <a name="input_sso_email"></a> [sso\_email](#input\_sso\_email) | The email address of the Control Tower SSO account | `string` | n/a | yes |
| <a name="input_provisioned_product_name"></a> [provisioned\_product\_name](#input\_provisioned\_product\_name) | A custom name for the provisioned product | `string` | `null` | no |
| <a name="input_sso_firstname"></a> [sso\_firstname](#input\_sso\_firstname) | The first name of the Control Tower SSO account | `string` | `"AWS Control Tower"` | no |
| <a name="input_sso_lastname"></a> [sso\_lastname](#input\_sso\_lastname) | The last name of the Control Tower SSO account | `string` | `"Admin"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id"></a> [id](#output\_id) | The AWS account ID |
| <a name="output_name"></a> [name](#output\_name) | The AWS account name |
<!-- END_TF_DOCS -->