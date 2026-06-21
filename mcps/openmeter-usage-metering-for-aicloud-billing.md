# OpenMeter (Usage Metering for AI/Cloud Billing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openmeter-usage-metering-for-aicloud-billing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openmeter-usage-metering-for-aicloud-billing-mcp)
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


## Installation & Usage

To install and use the **OpenMeter (Usage Metering for AI/Cloud Billing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
