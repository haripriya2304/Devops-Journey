# Day 6 – Creating AWS IAM User Using Terraform

## Overview

On Day 6 of my DevOps learning journey, I used **Terraform** to create an **AWS IAM User** using Infrastructure as Code (IaC).

The IAM user was successfully created by defining the AWS provider and IAM user resource in a Terraform configuration file.

## Objective

- Learn how Terraform works with AWS.
- Configure the AWS provider.
- Create an AWS IAM user using Terraform.
- Add tags to the IAM user.
- Understand the Terraform workflow.

## Technologies Used

- Terraform
- AWS IAM
- AWS Provider
- Infrastructure as Code (IaC)
- Visual Studio Code

## Project Structure

```text
Day6/
├── provider.tf
├── terraform.tfstate
├── terraform.tfstate.backup
└── .terraform.lock.hcl
