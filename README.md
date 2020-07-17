## Requirements

| Name | Version |
|------|---------|
| terraform | ~> 0.12.0 |
| yandex | ~> 0.41 |

## Providers

| Name | Version |
|------|---------|
| yandex | ~> 0.41 |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| description | An optional description of this resource. Provide this property when you create the resource. | `string` | `"Auto-created"` | no |
| name | Name to be used on all the resources as identifier | `string` | n/a | yes |
| subnets | n/a | <pre>list(object({<br>    zone           = string<br>    v4_cidr_blocks = list(string)<br>  }))</pre> | <pre>[<br>  {<br>    "v4_cidr_blocks": [<br>      "10.130.0.0/24"<br>    ],<br>    "zone": "ru-central1-a"<br>  },<br>  {<br>    "v4_cidr_blocks": [<br>      "10.129.0.0/24"<br>    ],<br>    "zone": "ru-central1-b"<br>  },<br>  {<br>    "v4_cidr_blocks": [<br>      "10.128.0.0/24"<br>    ],<br>    "zone": "ru-central1-c"<br>  }<br>]</pre> | no |

## Outputs

| Name | Description |
|------|-------------|
| network\_id | The ID of the VPC |
| subnet\_ids | n/a |
| subnet\_zones | n/a |

