# main.tf
terraform {
  required_providers {
    random = {
      source = "hashicorp/random"
      version = "~> 3.0"
    }
  }
}

provider "random" {}

resource "random_pet" "example" {
  length = 2
}

