# Improvement backlog

Items accepted for later work. Each item names its origin and the condition to start it.

| Id | Item | Origin | Start when |
|---|---|---|---|
| IB-01 | Replicate the AWS infrastructure of spec 001 with Terraform + Terragrunt (dev and prod, multi-region hierarchy under `aws/terraform/environments/<env>/<region>/...`), keeping parity with the SAM templates and a single `IAC_TOOL` switch (`sam` default, `terraform`) in the deployment workflows, as in over-engineered-simple-calculator-aws-sls-version. | Owner request, 2026-11-12 | Spec 001 deployed and verified in dev |
| IB-02 | Azure replica of this backend (compute on Azure Virtual Machine Scale Sets with autoscale) under the reserved `azure/` root, starting with a migration brief of this repository. | Owner request, 2026-11-12 | Spec 001 closed; IB-01 recommended first so both clouds share Terraform |
