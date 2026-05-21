# AI Agents

This folder will contain prompts, tool definitions, guardrails, and agent logic.

## Agent Types

### 1. Inventory Agent
Analyzes sales and inventory data to recommend restock or prep quantities.

### 2. Daily Business Agent
Creates a plain-English daily summary for the owner.

### 3. Phone Order Agent
Collects order details from customer calls and creates order drafts.

### 4. Marketing Agent
Drafts simple promotional messages based on sales trends.

## Core Principle

Agents should recommend and draft actions. They should not perform risky actions automatically.

## Example Agent Tools

```text
get_sales_history()
get_product_list()
get_current_inventory()
forecast_demand()
recommend_restock()
check_menu_item()
check_pickup_availability()
calculate_order_total()
create_order_draft()
notify_owner()
```

## Guardrails

Agents must:
- Use business-approved product, price, and policy data
- Ask for missing order details
- Avoid making promises outside company policy
- Avoid revealing customer private information
- Create drafts instead of confirming risky actions
