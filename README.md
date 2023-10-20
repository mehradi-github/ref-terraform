# Vagrant and Terraform

[Vagrant](https://developer.hashicorp.com/vagrant/tutorials/getting-started/getting-started-install) is a tool for building complete development environments. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases development/production parity, and makes the "it works on my machine" excuse a relic of the past.

[Terraform ](https://developer.hashicorp.com/terraform/downloads)is an infrastructure as code tool that lets you build, change, and version cloud and on-prem resources safely and efficiently.

- [Vagrant and Terraform](#vagrant-and-terraform)
  - [Install Vagrant](#install-vagrant)
  - [Install Terraform](#install-terraform)

## Install Vagrant

```sh
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install vagrant
```

## Install Terraform

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
