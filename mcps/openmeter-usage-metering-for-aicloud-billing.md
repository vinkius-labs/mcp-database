# OpenMeter (Usage Metering for AI/Cloud Billing) MCP Server

Meter AI usage, manage customer entitlements, and automate cloud billing via OpenMeter's high-performance usage tracking API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 9

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


## Installation & Usage

To install and use the **OpenMeter (Usage Metering for AI/Cloud Billing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing](https://vinkius.com/mcp/openmeter-usage-metering-for-aicloud-billing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
