# Color definitions for Terraform

This module provides static color definitions for Terraform.

## How to use?

```hcl
module "colors" {
  source  = "multani/colors/standard"
  version = "0.0.2"
}

output "green_web" {
  value = "#${module.colors.css.green}"
}
```

Will output:

```
Outputs:

green_web = "#008000"
```
