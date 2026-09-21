## Decision and Reasoning

CloudMedic decides whether recognizable infrastructure-as-code evidence exists for cloud deployment. When no Terraform or CloudFormation-style artifact is detected, it reports the structural gap.

## Inputs and Data Sources

It uses repository filenames and directory names as evidence, looking for terraform or cloudformation signals. The decision is deterministic and repository-scoped.

## Limits and Constraints

It does not assess cloud architecture, cost, IAM correctness, drift, or production readiness. Other infrastructure systems may be valid but remain outside the recognized evidence set.
