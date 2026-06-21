# Recharge MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recharge-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/recharge-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/recharge-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage subscription commerce via Recharge — handle customers, subscriptions, addresses, and delivery schedules directly from your AI agent.

## Description
Connect your **Recharge** account to any AI agent to streamline your subscription operations and customer management through natural conversation.

### What you can do

- **Customer Profiles** — Create, retrieve, and update customer records, including credit summaries and delivery schedules.
- **Subscription Management** — Fetch detailed subscription data to track recurring orders and customer status.
- **Address & Logistics** — Manage shipping addresses, merge duplicate records, and update delivery locations.
- **Operational Control** — Skip future charges for specific addresses and manage child resources for customer accounts.
- **Data Analysis** — List and sort customers or addresses to generate reports on your subscription base.

### How it works

1. Subscribe to this server
2. Enter your Recharge API Access Token
3. Start managing your recurring revenue directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check customer delivery schedules and subscription statuses without leaving your workflow.
- **Support Teams** — update shipping addresses or skip charges for customers instantly during a chat.
- **Operations Leads** — analyze customer lists and credit summaries to monitor business health.


## Available Tools
- **activate_subscription**: Reactivate a cancelled subscription
- **add_async_batch_tasks**: Add tasks to an async batch
- **apply_charge_discount**: Apply a discount to a queued charge
- **bulk_manage_product_plans**: Bulk manage plans for a product
- **cancel_subscription**: Cancel a subscription
- **change_subscription_address**: Update the associated address for a subscription
- **clone_order**: Clone an order for prepaid subscriptions
- **create_address**: Create a new address
- **create_async_batch**: Create an async batch
- **create_checkout**: Create a checkout
- **create_customer**: Create a customer
- **create_metafield**: Create a metafield
- **create_payment_method**: Create a payment method
- **create_plan**: Create a plan
- **create_product**: Create a product
- **create_subscription**: Create a subscription
- **create_webhook**: Create a webhook
- **delay_order**: Delay a prepaid order by one interval
- **delete_address**: Only works if there are no active subscriptions.

Delete an address
- **delete_customer**: Delete a customer and all child resources
- **delete_metafield**: Delete a metafield
- **delete_order**: Delete a scheduled order
- **delete_payment_method**: Delete a payment method
- **delete_plan**: Delete a plan
- **delete_product**: Delete a product
- **delete_subscription**: Delete a subscription
- **delete_webhook**: Delete a webhook
- **get_address**: Retrieve an address
- **get_async_batch**: Retrieve an async batch
- **get_charge**: Retrieve a charge
- **get_checkout_shipping_rates**: Retrieve available shipping rates for a checkout
- **get_checkout**: Retrieve a checkout
- **get_customer_credit_summary**: Retrieve credit balance for a customer
- **get_customer_delivery_schedule**: Retrieve projected deliveries for a customer
- **get_customer**: Retrieve a customer
- **get_metafield**: Retrieve a metafield
- **get_order**: Retrieve an order
- **get_payment_method**: Retrieve a payment method
- **get_plan**: Retrieve a plan
- **get_product**: Retrieve a product
- **get_subscription**: Retrieve a subscription
- **get_webhook**: Retrieve a webhook
- **list_addresses**: List addresses
- **list_charges**: List charges
- **list_customers**: List customers
- **list_metafields**: List metafields
- **list_orders**: List orders
- **list_plans**: List plans
- **list_subscriptions**: List subscriptions
- **merge_addresses**: Merge up to 10 source addresses into 1 target
- **process_async_batch**: Process an async batch
- **process_charge**: Manually process a queued charge
- **process_checkout**: Process the checkout
- **refund_charge**: Refund a processed charge
- **remove_charge_discount**: Remove a discount from a charge
- **set_subscription_next_charge_date**: Change the next charge date for a subscription
- **skip_address_charges**: Skip a future charge for specific subscriptions on an address
- **skip_charge**: Skip a charge
- **test_webhook**: Test a webhook
- **unskip_charge**: Unskip a charge
- **update_address**: Update an address
- **update_checkout**: Update a checkout
- **update_customer**: Update a customer
- **update_metafield**: Update a metafield
- **update_order**: Update an order
- **update_payment_method**: Update a payment method
- **update_plan**: Update a plan
- **update_product**: Update a product
- **update_subscription**: Update a subscription
- **update_webhook**: Update a webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recharge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent 10 customers from Recharge."

**🤖 AI Agent:**
> I've retrieved the latest customers. The list includes 'Jane Doe' (ID: 88231), 'John Smith' (ID: 88232), and 8 others. Would you like to see the details for a specific customer?

---

**👤 You:**
> "Show me the delivery schedule for customer 123456."

**🤖 AI Agent:**
> Fetching the schedule for customer 123456... They have 3 upcoming deliveries: June 15th (Monthly Coffee), July 15th (Monthly Coffee), and August 15th (Monthly Coffee).

---

**👤 You:**
> "Get the details for subscription ID 998877."

**🤖 AI Agent:**
> Inspecting subscription 998877... It is an active 'Premium Skincare Bundle' priced at $45.00, renewing every 30 days. The next charge date is set for June 20th.


## Installation & Usage

To install and use the **Recharge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recharge-alternative](https://vinkius.com/mcp/recharge-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
