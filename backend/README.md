# Backend

This folder will contain APIs, database logic, authentication, and integrations.

## Suggested Stack

- FastAPI or Node.js/Express
- PostgreSQL or Supabase
- Python data processing for forecasting
- API routes for dashboard, inventory, orders, agents, and approvals

## Main Responsibilities

The backend should:
- Store business profiles
- Store product and sales data
- Process CSV uploads
- Generate sales summaries
- Create inventory recommendations
- Save phone order drafts
- Track approval status
- Keep an audit log of agent actions

## Suggested API Endpoints

```text
POST /upload-sales-csv
GET /dashboard-summary
GET /products
GET /recommendations
POST /orders/draft
POST /approvals/:id/approve
POST /approvals/:id/reject
GET /agent-activity
```

## Backend Safety Rules

The backend should enforce safety rules, not just the frontend.

Important actions should require owner approval:
- Confirming orders
- Sending customer messages
- Changing inventory
- Charging payments
- Placing supplier orders
