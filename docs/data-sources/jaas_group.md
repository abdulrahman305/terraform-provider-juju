---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "juju_jaas_group Data Source - terraform-provider-juju"
subcategory: ""
description: |-
  A data source representing a Juju JAAS Group.
---

# juju_jaas_group (Data Source)

A data source representing a Juju JAAS Group.

## Example Usage

```terraform
data "juju_jaas_group" "test" {
  name = "group-0"
}

output "group_uuid" {
  value = data.juju_jaas_group.test.uuid
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The name of the group.

### Read-Only

- `uuid` (String) The UUID of the group.