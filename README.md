# terraform-cloudatcost
cloudatcost provider terraform

## References
https://github.com/cloudatcost/api
github.com/masayukioguni/go-cloudatcost/cloudatcost
github.com/Blackturtle123/go-cloudatcost/cloudatcost

## Example
```
provider "cloudatcost" {
  api_key     = "key"
  login       = "email"
}

resource "cloudatcost_machine" "servera" {
  "cpu"="1",
  "ram"="512",
  "storage"="10",
  "os"="26",
  "datacenter"="Developer-DC-2",
}

resource "cloudatcost_machine" "serverb" {
  "cpu"="1",
  "ram"="512",
  "storage"="20",
  "os"="26",
  "datacenter"="Developer-DC-2",
}
```