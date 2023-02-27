# Color definitions for Terraform

This module provides static color definitions for Terraform.

You can refer to the following color names to get the related color:

* [CSS: Basic colors](https://www.w3.org/TR/css-color-3/#html4)
* [CSS: Extended colors](https://www.w3.org/TR/css-color-3/#svg-color)



## How to use?

```hcl
module "colors" {
  source  = "multani/colors/standard"
  version = "0.0.3"
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
