# Specialist Draft: Cloud Architect
**Target**: AWS Scalable Infrastructure for AI Agents

## 1. Compute Layer
*   **AWS EKS (Kubernetes)**: Deployment of agent containers with HPA (Horizontal Pod Autoscaler) triggered by CPU/Memory and custom LLM latency metrics.
*   **Spot Instances**: Utilizing Spot Ocean for cost-optimization during non-peak, switching to On-Demand for Black Friday.

## 2. Data Strategy
*   **RDS Proxy**: Ensuring the Agent system doesn't overwhelm the SQL database with connection spikes.
*   **ElastiCache (Redis)**: Storing agent session state for rapid retrieval.

## 3. Scalability
*   **Global Accelerator**: Reducing latency for international customers.
