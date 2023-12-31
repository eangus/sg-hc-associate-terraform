# Study guide for HashiCorp's Associate Terraform

[Exam Details](https://www.hashicorp.com/certification/terraform-associate)

[Ojective Docs](https://developer.hashicorp.com/terraform/tutorials/certification-003/associate-review-003)

## Exam objectives

1. [Understand infrastructure as code (IaC) concepts](#1-understand-infrastructure-as-code-iac-concepts)
	- 1a. [Explain what IaC is](#1a-explain-what-iac-is)
	- 1b. [Describe advantages of IaC patterns](#1b-describe-advantages-of-iac-patterns)
2. [Understand the purpose of Terraform (vs other IaC)](#2-understand-the-purpose-of-terraform-vs-other-iac)
	- 2a. [Explain multi-cloud and provider-agnostic benefits](#2a-explain-multi-cloud-and-provider-agnostic-benefits)
	- 2b. [Explain the benefits of state](#2b-explain-the-benefits-of-state)
3. [Understand Terraform basics](#3-understand-terraform-basics)
	- 3a. [Install and version Terraform providers](#3a-install-and-version-terraform-providers)
	- 3b. [Describe plugin-based architecture](#3b-describe-plugin-based-architecture)
	- 3c. [Write Terraform configuration using multiple providers](#3c-write-terraform-configuration-using-multiple-providers)
	- 3d. [Describe how Terraform finds and fetches providers](#3d-describe-how-terraform-finds-and-fetches-providers)
4. [Use Terraform outside of core workflow](#4-use-terraform-outside-of-core-workflow)
	- 4a. [Describe when to use terraform import to import existing infrastructure into your Terraform state](#4a-describe-when-to-use-terraform-import-to-import-existing-infrastructure-into-your-terraform-state)
	- 4b. [Use terraform state to view Terraform state](#4b-use-terraform-state-to-view-terraform-state)
	- 4c. [Describe when to enable verbose logging and what the outcome/value is](#4c-describe-when-to-enable-verbose-logging-and-what-the-outcomevalue-is)
5. [Interact with Terraform modules](#5-interact-with-terraform-modules)
	- 5a. [Contrast and use different module source options including the public Terraform Module Registry](#5a-contrast-and-use-different-module-source-options-including-the-public-terraform-module-registry)
	- 5b. [Interact with module inputs and outputs](#5b-interact-with-module-inputs-and-outputs)
	- 5c. [Describe variable scope within modules/child modules](#5c-describe-variable-scope-within-moduleschild-modules)
	- 5d. [Set module version](#5d-set-module-version)
6. [Use the core Terraform workflow](#6-use-the-core-terraform-workflow)
	- 6a. [Describe Terraform workflow ( Write -> Plan -> Create )](#6a-describe-terraform-workflow--write---plan---create-)
	- 6b. [Initialize a Terraform working directory (terraform init)](#6b-initialize-a-terraform-working-directory-terraform-init)
	- 6c. [Validate a Terraform configuration (terraform validate)](#6c-validate-a-terraform-configuration-terraform-validate)
	- 6d. [Generate and review an execution plan for Terraform (terraform plan)](#6d-generate-and-review-an-execution-plan-for-terraform-terraform-plan)
	- 6e. [Execute changes to infrastructure with Terraform (terraform apply)](#6e-execute-changes-to-infrastructure-with-terraform-terraform-apply)
	- 6f. [Destroy Terraform managed infrastructure (terraform destroy)](#6f-destroy-terraform-managed-infrastructure-terraform-destroy)
	- 6g. [Apply formatting and style adjustments to a configuration (terraform fmt)](#6g-apply-formatting-and-style-adjustments-to-a-configuration-terraform-fmt)
7. [Implement and maintain state](#7-implement-and-maintain-state)
	- 7a. [Describe default local backend](#7a-describe-default-local-backend)
	- 7b. [Describe state locking](#7b-describe-state-locking)
	- 7c. [Handle backend and cloud integration authentication methods](#7c-handle-backend-and-cloud-integration-authentication-methods)
	- 7d. [Differentiate remote state back end options](#7d-differentiate-remote-state-back-end-options)
	- 7e. [Manage resource drift and Terraform state](#7e-manage-resource-drift-and-terraform-state)
	- 7f. [Describe backend block and cloud integration in configuration](#7f-describe-backend-block-and-cloud-integration-in-configuration)
	- 7g. [Understand secret management in state files](#7g-understand-secret-management-in-state-files)
8. [Read, generate, and modify configuration](#8-read,-generate,-and-modify-configuration)
	- 8a. [Demonstrate use of variables and outputs](#8a-demonstrate-use-of-variables-and-outputs)
	- 8b. [Describe secure secret injection best practice](#8b-describe-secure-secret-injection-best-practice)
	- 8c. [Understand the use of collection and structural types](#8c-understand-the-use-of-collection-and-structural-types)
	- 8d. [Create and differentiate resource and data configuration](#8d-create-and-differentiate-resource-and-data-configuration)
	- 8e. [Use resource addressing and resource parameters to connect resources together](#8e-use-resource-addressing-and-resource-parameters-to-connect-resources-together)
	- 8f. [Use HCL and Terraform functions to write configuration](#8f-use-hcl-and-terraform-functions-to-write-configuration)

---

## 1 Understand infrastructure as code (IaC) concepts
### 1a Explain what IaC is
### 1b Describe advantages of IaC patterns
## 2 Understand the purpose of Terraform (vs other IaC)
### 2a Explain multi-cloud and provider-agnostic benefits
### 2b Explain the benefits of state
## 3 Understand Terraform basics
### 3a Install and version Terraform providers
### 3b Describe plugin-based architecture
### 3c Write Terraform configuration using multiple providers
### 3d Describe how Terraform finds and fetches providers
## 4 Use Terraform outside of core workflow
### 4a Describe when to use terraform import to import existing infrastructure into your Terraform state
### 4b Use terraform state to view Terraform state
### 4c Describe when to enable verbose logging and what the outcome/value is
## 5 Interact with Terraform modules
### 5a Contrast and use different module source options including the public Terraform Module Registry
### 5b Interact with module inputs and outputs
### 5c Describe variable scope within modules/child modules
### 5d Set module version
## 6 Use the core Terraform workflow
### 6a Describe Terraform workflow ( Write -> Plan -> Create )
### 6b Initialize a Terraform working directory (terraform init)
### 6c Validate a Terraform configuration (terraform validate)
### 6d Generate and review an execution plan for Terraform (terraform plan)
### 6e Execute changes to infrastructure with Terraform (terraform apply)
### 6f Destroy Terraform managed infrastructure (terraform destroy)
### 6g Apply formatting and style adjustments to a configuration (terraform fmt)
## 7 Implement and maintain state
### 7a Describe default local backend
### 7b Describe state locking
### 7c Handle backend and cloud integration authentication methods
### 7d Differentiate remote state back end options
### 7e Manage resource drift and Terraform state
### 7f Describe backend block and cloud integration in configuration
### 7g Understand secret management in state files
## 8 Read, generate, and modify configuration
### 8a Demonstrate use of variables and outputs
### 8b Describe secure secret injection best practice
### 8c Understand the use of collection and structural types
### 8d Create and differentiate resource and data configuration
### 8e Use resource addressing and resource parameters to connect resources together
### 8f Use HCL and Terraform functions to write configuration
