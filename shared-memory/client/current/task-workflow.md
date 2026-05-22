# Specialist Draft: Workflow Automator
**Target**: ReAct-based Customer Support Agentic Loop

## 1. Orchestration
*   **ReAct Loop**: Implementation of "Reason + Act" pattern. The agent will first check the SQL database (Reason) and then decide whether to call the Return API (Act).
*   **Tool Schema**: Standardized JSON-RPC schemas for `get_order_status` and `initiate_return`.

## 2. Recommendation Logic
*   **Vector DB (Pinecone/Milvus)**: If an item is out of stock, the agent performs a similarity search on product embeddings to suggest alternatives.

## 3. Human-in-the-loop
*   **Escalation Trigger**: If confidence score < 0.8 or sentiment is "Angry", the workflow automatically creates a Zendesk ticket.
