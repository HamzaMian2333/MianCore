# Intern Onboarding

Welcome to the MianCore project.

## What We Are Building

MianCore is an AI operations dashboard for small businesses. The first target market is bakeries, cafés, dessert shops, and other small food businesses.

The product helps owners:
- Understand sales
- Know what to restock
- Know what to prepare
- Review AI-created phone orders
- Approve important actions before they happen

## Product Principle

The AI should act like an assistant, not the owner.

It can:
- Recommend
- Summarize
- Draft
- Flag risks

The owner approves anything important.

## First Things to Read

Before starting work, read:

1. `README.md`
2. `docs/product-requirements.md`
3. `docs/architecture.md`
4. `docs/agent-safety-rules.md`
5. `CONTRIBUTING.md`

## How to Pick Work

1. Go to GitHub Issues.
2. Pick an issue labeled `good-first-issue`, `frontend`, `backend`, `ai-agent`, `data`, or `documentation`.
3. Comment on the issue that you are working on it.
4. Create a branch.
5. Open a pull request when done.

## Branch Rules

Do not work directly on `main`.

Use names like:

```text
feature/dashboard-ui
feature/csv-upload
feature/recommendation-cards
docs/update-roadmap
research/twilio
```

## Pull Request Checklist

Before opening a pull request:

- Code runs locally
- No API keys committed
- README updated if needed
- Screenshots added for UI changes
- Testing steps included
- Known issues mentioned

## Suggested First Tasks

Frontend:
- Dashboard layout
- Revenue chart
- Product sales table
- Approval queue UI

Backend:
- CSV upload endpoint
- Product/sales data model
- Recommendation endpoint
- Order draft endpoint

AI Agents:
- Daily summary prompt
- Restock recommendation prompt
- Agent safety guardrails

Data:
- Create more sample CSV datasets
- Test recommendation logic with fake data

Research:
- Twilio voice integration
- Square API integration
- Shopify API integration
