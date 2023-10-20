# Terraform

[Terraform ](https://developer.hashicorp.com/terraform/downloads)is an infrastructure as code tool that lets you build, change, and version cloud and on-prem resources safely and efficiently.

- [Terraform](#terraform)
  - [Install](#install)

## Install

```sh
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform

terraform version
```

Syntax highlighting and autocompletion for Terraform via [HashiCorp Terraform](https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform)

Launch VS Code:

```sh
ext install HashiCorp.terraform
```
