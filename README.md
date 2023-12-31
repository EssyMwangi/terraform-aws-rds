## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.2.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 4.15.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.15.1 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_db_instance.primary](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/db_instance) | resource |
| [aws_db_instance.read_replica](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/db_instance) | resource |
| [aws_db_subnet_group.rds_subnet_group](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/db_subnet_group) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_allocated_storage"></a> [allocated\_storage](#input\_allocated\_storage) | Allocated Storage in gigabytes | `number` | n/a | yes |
| <a name="input_db_engine"></a> [db\_engine](#input\_db\_engine) | Database Engine to Use e.g postgres,msql | `string` | n/a | yes |
| <a name="input_db_engine_version"></a> [db\_engine\_version](#input\_db\_engine\_version) | Version of DB engine e.g 5.7 for mySQL 5.7 | `string` | n/a | yes |
| <a name="input_db_instance_class"></a> [db\_instance\_class](#input\_db\_instance\_class) | The AWS instance type to use for the RDS instance | `string` | n/a | yes |
| <a name="input_db_password"></a> [db\_password](#input\_db\_password) | Credentials for Accessing RDS Instance | `string` | n/a | yes |
| <a name="input_multi_az"></a> [multi\_az](#input\_multi\_az) | If The RDS should be run in multi\_az | `bool` | n/a | yes |
| <a name="input_parameter_group_name"></a> [parameter\_group\_name](#input\_parameter\_group\_name) | Parameter Group to associate with the RDS e.g default.mysql5.7 | `string` | n/a | yes |
| <a name="input_project"></a> [project](#input\_project) | Project Name | `string` | n/a | yes |
| <a name="input_region"></a> [region](#input\_region) | default region for resources | `string` | n/a | yes |
| <a name="input_skip_final_snapshot"></a> [skip\_final\_snapshot](#input\_skip\_final\_snapshot) | Setting this to true means that no final DB snapshot is created when the RDS instance is deleted. | `bool` | n/a | yes |
| <a name="input_storage_type"></a> [storage\_type](#input\_storage\_type) | type of storage to use e.g gp2,standard | `string` | n/a | yes |
| <a name="input_subnet_ids"></a> [subnet\_ids](#input\_subnet\_ids) | RDS Variables | `list(string)` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | Tags for resources | `map(string)` | n/a | yes |
| <a name="input_username"></a> [username](#input\_username) | Credentials for Accessing RDS Instance | `string` | n/a | yes |
| <a name="input_vpc_security_group_id"></a> [vpc\_security\_group\_id](#input\_vpc\_security\_group\_id) | Security Group to Associate with the RDS | `string` | n/a | yes |

## Outputs

No outputs.
