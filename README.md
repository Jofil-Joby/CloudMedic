# CloudMedic

> Portable agent for identifying missing recognizable cloud infrastructure configuration.

## What it does

CloudMedic looks for infrastructure-as-code evidence such as Terraform or CloudFormation and reports when no recognizable cloud configuration is present.

### Diagnostic fingerprint

**Infrastructure evidence → cloud-readiness signal → explanation → next step**

## Why this agent is distinct

CloudMedic is deliberately narrower than a general cloud security or architecture scanner. Its question is whether the repository exposes an inspectable infrastructure definition.

That makes it useful as a discovery layer before deeper cloud analysis.

## Workflow

```text
Repository
    ↓
IaC detector
    ↓
Cloud configuration rule
    ↓
Evidence-backed finding
    ↓
Infrastructure recommendation
```

## Verification

The repository provides OpenGAP passport metadata, cloud-focused fixture coverage, explainability contracts, four framework adapters, and automated adapter verification.

OpenGAP validation passed and all four generated exports have been exercised successfully.

## Design principle

**Infrastructure should be observable.** CloudMedic reports visible repository evidence and avoids inventing deployment architecture that is not present.

## Medic family

CloudMedic adds a focused infrastructure perspective to the portable Medic family.