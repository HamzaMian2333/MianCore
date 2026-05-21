# Architecture

## High-Level System

```text
Business Data
CSV / Google Sheets / Square / Shopify
        ↓
Backend API
Data validation, business logic, authentication
        ↓
Database
Products, sales, inventory, orders, approvals, agent activity
        ↓
Analytics Layer
Pandas / forecasting / trend detection
        ↓
AI Agent Layer
Summaries, recommendations, order drafts
        ↓
Dashboard
Owner reviews insights and approvals
```

## MVP Architecture

For the first version:

```text
CSV Upload
    ↓
Backend parses file
    ↓
Sales data stored in database
    ↓
Analytics generates metrics
    ↓
AI agent writes summary
    ↓
Dashboard displays recommendations
    ↓
Owner approves/rejects drafts
```

## Main Components

### Frontend

Responsible for:
- Login page
- Dashboard
- CSV upload
- Charts
- Recommendation cards
- Approval queue
- Order draft cards

### Backend

Responsible for:
- API endpoints
- CSV processing
- Database operations
- Business rules
- Agent tool calls
- Approval workflow

### Database

Stores:
- Users
- Businesses
- Products
- Sales
- Inventory
- Orders
- Recommendations
- Approvals
- Agent activity logs

### AI Agents

Responsible for:
- Daily summary
- Inventory recommendations
- Phone order draft generation
- Marketing draft suggestions

### Integrations Later

Possible integrations:
- Twilio for voice calls
- Square for POS/order data
- Shopify for e-commerce data
- Stripe for payment links
- Google Sheets for manual data sync

## Safety Architecture

Safety should exist at multiple layers:

1. Frontend displays approval controls.
2. Backend blocks risky actions without approval.
3. AI agents follow guardrails.
4. Audit logs track what happened.
5. Owner can edit or reject every important action.

## Important Design Rule

Do not depend only on AI reasoning for business-critical decisions.

Use deterministic logic for numbers:
- Sales totals
- Inventory counts
- Revenue
- Forecast inputs
- Order totals

Use AI for:
- Explanation
- Summarization
- Recommendations
- Drafting messages
