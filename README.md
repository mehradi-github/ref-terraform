# Vagrant and Terraform

[Vagrant](https://developer.hashicorp.com/vagrant/tutorials/getting-started/getting-started-install) is a tool for building complete development environments. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases development/production parity, and makes the "it works on my machine" excuse a relic of the past.

[Terraform ](https://developer.hashicorp.com/terraform/downloads)is an infrastructure as code tool that lets you build, change, and version cloud and on-prem resources safely and efficiently.

- [Vagrant and Terraform](#vagrant-and-terraform)
  - [Vagrant vs. Terraform](#vagrant-vs-terraform)
  - [Install Vagrant](#install-vagrant)
  - [Install Terraform](#install-terraform)

## [Vagrant vs. Terraform](https://developer.hashicorp.com/vagrant/intro/vs/terraform)

Vagrant is a tool focused for managing development environments and Terraform is a tool for building infrastructure.

The primary usage of Terraform is for managing remote resources in cloud providers such as AWS. Terraform is designed to be able to manage extremely large infrastructures that span multiple cloud providers. Vagrant is designed primarily for local development environments that use only a handful of virtual machines at most.

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
