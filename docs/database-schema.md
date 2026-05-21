# Database Schema

This is a starter schema for the MVP.

## users

Stores account information.

```text
id
name
email
role
created_at
```

## businesses

Stores small business profiles.

```text
id
owner_user_id
business_name
business_type
phone_number
timezone
created_at
```

## products

Stores products sold by the business.

```text
id
business_id
name
category
price
is_active
created_at
```

## sales

Stores sales records.

```text
id
business_id
product_id
date
quantity_sold
revenue
source
created_at
```

## inventory

Stores current inventory or prep count.

```text
id
business_id
product_id
inventory_on_hand
reorder_threshold
last_updated
```

## recommendations

Stores AI/data-generated recommendations.

```text
id
business_id
recommendation_type
title
description
reason
risk_level
status
created_at
```

Example recommendation types:
- restock
- reduce_inventory
- prep_quantity
- marketing
- alert

Example statuses:
- pending
- approved
- rejected
- edited

## orders

Stores phone or dashboard order drafts.

```text
id
business_id
customer_name
customer_phone
order_details
estimated_total
pickup_datetime
status
source
created_at
```

Example statuses:
- draft
- needs_approval
- approved
- rejected
- completed

## approvals

Tracks owner approvals.

```text
id
business_id
related_entity_type
related_entity_id
action_requested
status
approved_by
approved_at
created_at
```

## agent_activity_logs

Tracks what agents did.

```text
id
business_id
agent_name
activity_type
input_summary
output_summary
risk_level
created_at
```

## call_transcripts Later

For phone order agent.

```text
id
business_id
order_id
customer_phone
transcript_text
call_duration_seconds
created_at
```

## Notes

For the MVP, start simple. Do not overbuild the schema before testing the product.
