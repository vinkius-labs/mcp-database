# OpenMeter (Usage Metering for AI/Cloud Billing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Meter AI usage, manage customer entitlements, and automate cloud billing via OpenMeter's high-performance usage tracking API.

## Description
Connect **OpenMeter** to your AI agent to handle complex usage-based billing and entitlement management for AI and Cloud services through natural language.

### What you can do

- **Usage Ingestion** — Send usage events (like token counts or API calls) in CloudEvents format directly to your metering pipeline
- **Customer Management** — Create and retrieve billable customer profiles, mapping them to internal keys or subjects
- **Entitlements & Features** — Define metered features and set specific usage limits or access rights for each customer
- **Subscription Orchestration** — Link customers to plans and manage the lifecycle of their subscriptions
- **Payment Integration** — Initiate Stripe checkout sessions for seamless payment collection and subscription starts

### How it works

1. Subscribe to this server
2. Enter your OpenMeter API Key
3. Start metering and billing your AI users directly from your agent

Your AI now acts as a billing operations specialist, capable of tracking consumption and managing access without manual dashboard intervention.

### Who is this for?

- **SaaS Founders** — automate the transition from usage to invoice by letting the AI handle event ingestion and customer setup
- **FinOps Teams** — query customer consumption and entitlement status using natural language
- **Product Engineers** — define new features and metered resources directly from the development environment


## Available Tools
- **create_customer**: Create a new billable customer
- **create_entitlement**: Create an entitlement for a customer
- **create_feature**: Create a new feature for metering
- **create_stripe_checkout**: Create a Stripe checkout session
- **create_subscription**: Create a subscription
- **delete_subject**: Delete a subject by key
- **get_customer**: Get a customer by ID or Key
- **ingest_event**: Ingest a usage event into OpenMeter
- **upsert_subjects**: Provide an array of subject objects.

Upsert subjects in OpenMeter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenMeter (Usage Metering for AI/Cloud Billing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ingest a 'tokens' event for subject 'cust_99' with 150 tokens from source 'gpt-wrapper'."

**🤖 AI Agent:**
> I've successfully ingested the usage event. Event ID: `evt_01H...`. 150 tokens have been recorded for customer `cust_99`.

---

**👤 You:**
> "Create a new feature called 'Image Generation' with key 'img_gen' and meter slug 'images_total'."

**🤖 AI Agent:**
> Feature 'Image Generation' (img_gen) has been created and linked to the 'images_total' meter. You can now assign entitlements for this feature to your customers.

---

**👤 You:**
> "Get the details for customer with key 'acme-corp-001'."

**🤖 AI Agent:**
> Retrieved customer: ACME Corp (ID: `cust_abc123`). Usage is attributed to subjects: `['acme-corp-001']`.


## ❓ FAQ

**Q: How do I record that a user just consumed 500 tokens in an AI prompt?**
Use the `ingest_event` tool. Provide the event type (e.g., 'prompt'), the subject (customer ID), and a JSON payload containing the count (e.g., `{"tokens": 500}`). OpenMeter will handle the aggregation automatically.

**Q: Can I check the current status and metadata of a specific billable customer?**
Yes! Use the `get_customer` tool with the customer's ID or Key. It will return the customer's name, usage attribution settings, and internal identifiers.

**Q: How do I set a usage limit or entitlement for a customer?**
Use the `create_entitlement` tool. You'll need the `customerId` and a JSON configuration defining the feature and the limit (e.g., a hard limit of 1000 units per month).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenMeter (Usage Metering for AI/Cloud Billing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `openmeter-usage-metering-for-aicloud-billing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenMeter (Usage Metering for AI/Cloud Billing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openmeter-usage-metering-for-aicloud-billing": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
