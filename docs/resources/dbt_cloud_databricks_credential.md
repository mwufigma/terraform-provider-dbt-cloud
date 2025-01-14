---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "dbt_cloud_databricks_credential Resource - terraform-provider-dbt-cloud"
subcategory: ""
description: |-
  
---

# dbt_cloud_databricks_credential (Resource)



## Example Usage

```terraform
resource "dbt_cloud_databricks_credential" "new_credential" {
  project_id  = data.dbt_cloud_project.test_project.project_id
  adapter_id  = 123
  num_threads = 16
  target_name = "MOO"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `adapter_id` (Number) Databricks adapter ID for the credential
- `num_threads` (Number) Number of threads to use
- `project_id` (Number) Project ID to create the Databricks credential in
- `target_name` (String) Target name
- `token` (String, Sensitive) Token for Databricks user

### Read-Only

- `credential_id` (Number) The system Databricks credential ID
- `id` (String) The ID of this resource.

## Import

Import is supported using the following syntax:

```shell
# Import using a project ID and credential ID found in the URL or via the API.
terraform import dbt_cloud_databricks_credential.test_databricks_credential "project_id:credential_id"
terraform import dbt_cloud_databricks_credential.test_databricks_credential 12345:6789
```
