# MianCore

MianCore is an AI operations dashboard for small businesses.

The platform helps business owners:
- View sales and inventory insights
- Get AI restock and prep recommendations
- Generate daily business summaries
- Manage AI-created phone order drafts
- Approve or reject important actions before they happen

## Product Principle

The AI can recommend, summarize, and draft actions, but the business owner approves anything important.

## MVP Scope

### Phase 1: Dashboard + CSV Upload
- Upload sales CSV
- View revenue, top products, slow products
- Show inventory warnings
- Generate daily business summary

### Phase 2: Inventory Agent
- Recommend what to restock
- Recommend what to reduce
- Predict demand for the next few days
- Explain why the recommendation was made

### Phase 3: Approval Queue
- Owner approves/rejects/edit actions
- Track pending phone orders
- Keep an audit log of agent activity

### Phase 4: Phone Order Agent
- AI answers calls
- Collects customer order details
- Creates order draft
- Sends order to owner dashboard for approval

## Tech Stack

Frontend: React / Next.js  
Backend: FastAPI or Node.js  
Database: PostgreSQL / Supabase  
AI: OpenAI API / Agents SDK  
Voice: Twilio  
Data Analysis: Python, Pandas  

## Safety Rules

The agent should NOT:
- Charge payments automatically
- Confirm expensive orders without approval
- Change inventory without approval
- Send customer messages without approval
- Delete business data

## Folder Structure

```text
frontend/
backend/
ai-agents/
docs/
sample-data/
.github/
