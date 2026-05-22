# Client Brief: NextGen E-Commerce AI Transformation

## 1. Background
We are a medium-sized e-commerce platform specializing in sustainable fashion. Our customer support team is overwhelmed by repetitive queries (order tracking, return policies, product sizing). We want to implement an autonomous AI agent system to handle 70% of these queries.

## 2. Technical Requirements
- **Cloud Infrastructure**: Must be hosted on AWS (current stack). We need a scalable solution for peak seasons (Black Friday).
- **Agent Logic**: The agent should be able to check order status in our SQL database and initiate return labels via API. It needs to handle complex "agentic" reasoning (e.g., if a product is out of stock, suggest a similar item).
- **Security**: Customer data must be encrypted. The agent should only have read-only access to the database where possible. We need full audit logs of every agent action.

## 3. Constraints
- **Budget**: $50,000 for the initial infrastructure and workflow design.
- **Timeline**: 4 weeks for the prototype.
- **Mindset**: We are fully committed to AI-native operations and are willing to rethink our current rigid ticket-based support flow.
