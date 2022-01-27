# Introduction:

The goal of this module is to showcase to students how easy it is to get up and running with a Vault HA Cluster backed by Consul in just a few commands. We will be deploying this Vault cluster on AWS using Terraform.
Estimated Time to Complete:

30-45 Minutes
Solution:

Provision a quick start Vault & Consul cluster in a private network with a bastion host.
Prerequisites

    Download Terraform
    [Download AWS CLI] (https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)

We will now provision the Terraform Quick Start Vault & Consul clusters.
Step 1: Initialize

Initialize Terraform - download providers and modules.
CLI

terraform init Command
Request

$ terraform init

Response

Step 2: Plan

Run a terraform plan to ensure Terraform will provision what you expect.
CLI

terraform plan Command
Request

$ terraform plan

Response

Step 3: Apply

Run a terraform apply to provision the HashiStack. One provisioned, view the zREADME instructions output from Terraform for next steps.
CLI

terraform apply command
Request

$ terraform apply

Response

Reference Material

    Terraform Getting Started
    Terraform Docs
    Consul Getting Started
    Consul Docs
    Vault Getting Started
    Vault Docs
