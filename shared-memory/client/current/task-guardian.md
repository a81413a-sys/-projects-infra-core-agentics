# Specialist Draft: Compliance Guardian
**Target**: Zero-Trust Security & Observability

## 1. Access Control
*   **IAM Roles for Service Accounts (IRSA)**: The EKS pods will have temporary, scoped IAM roles.
*   **SQL Isolation**: Providing a dedicated read-only user for the Agent, restricted to specific tables (Orders, Inventory).

## 2. Encryption
*   **AWS KMS**: All PII (Personally Identifiable Information) in the session state will be encrypted at rest.

## 3. Auditability
*   **LangSmith / Weights & Biases Integration**: For tracing agent reasoning steps.
*   **CloudWatch Logs**: Centralized storage for all tool-call outputs for compliance audits.
