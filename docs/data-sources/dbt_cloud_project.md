---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "dbt_cloud_project Data Source - terraform-provider-dbt-cloud"
subcategory: ""
description: |-
  
---

# dbt_cloud_project (Data Source)



## Example Usage

```terraform
data "dbt_cloud_project" "test_project" {
  project_id = var.dbt_cloud_project_id
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `project_id` (Number) ID of the project to represent

### Read-Only

- `connection_id` (Number) ID of the connection associated with the project
- `id` (String) The ID of this resource.
- `name` (String) Given name for project
- `repository_id` (Number) ID of the repository associated with the project
- `state` (Number) Project state should be 1 = active, as 2 = deleted


