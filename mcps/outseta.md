# Outseta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/outseta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Launch your SaaS faster with billing, authentication, CRM, and email built into one platform that eliminates integration headaches.

## Description
Connect your **Outseta** account to any AI agent and take full control of your all-in-one SaaS orchestration through natural conversation. Outseta provides a unified platform for CRM, subscription billing, email marketing, and help desk, and this integration allows you to retrieve customer metadata, manage invoices, and respond to support tickets directly from your chat interface.

### What you can do

- **CRM & Audience Orchestration** — List all managed people and company accounts programmatically to ensure your customer database is always synchronized.
- **Billing & Subscription Management** — Access and monitor active subscriptions and retrieve detailed invoice metadata directly from the AI interface to track revenue health.
- **Support & Help Desk Control** — List and create support tickets via natural language to drive better customer satisfaction and faster response times.
- **Plan & Activity Intelligence** — Access your subscription plans and monitor account activities using simple AI commands to maintain a clear overview of your business growth.
- **Operational Monitoring** — Track system responses and manage user profile metadata to ensure your SaaS workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Outseta Subdomain, API Key, and Secret Key from your settings
3. Start managing your SaaS business from Claude, Cursor, or any MCP-compatible client

No more jumping between disparate tools for support and billing. Your AI acts as a dedicated SaaS operations lead or customer success coordinator.

### Who is this for?

- **SaaS Founders** — quickly retrieve profitability summaries and monitor churn without switching apps.
- **Customer Success Teams** — automate the management of support tickets and track account health via natural conversation.
- **Operations Managers** — streamline the retrieval of billing metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_person**: Provide email and optionally name.

Create a new person in the CRM
- **create_ticket**: Create a new support ticket
- **get_account**: Get details of a specific account
- **get_person**: Get details of a specific person
- **get_user_profile**: Get current user profile
- **list_accounts**: List all accounts (companies)
- **list_activities**: List recent activities
- **list_invoices**: List all billing invoices
- **list_people**: List all people (contacts/leads)
- **list_plans**: List all billing plans
- **list_subscriptions**: List all billing subscriptions
- **list_tickets**: List all support tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outseta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active people in my Outseta CRM."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 50 active people in your CRM. Notable recent profiles include 'John Miller' and 'Sarah Chen'. Which one would you like to see activity for?

---

**👤 You:**
> "Show me all subscribers whose billing failed this month and their plan details."

**🤖 AI Agent:**
> 12 subscribers have failed billing this month. 7 are on the Pro plan ($49/mo), 3 on Enterprise ($199/mo), and 2 on Starter ($19/mo). Total at-risk MRR is $1,071. The most common failure reason is expired credit cards (8 cases). 4 subscribers are past their 3rd retry attempt and may need manual outreach.

---

**👤 You:**
> "Create a new trial account for contact sarah@meridian.io on the Pro plan."

**🤖 AI Agent:**
> Trial account created successfully for sarah@meridian.io. Plan: Pro (14-day free trial). Account ID: acc_8421. A welcome email with login credentials has been sent. The trial will expire on May 27th, after which the account will convert to a paid subscription at $49/month unless cancelled.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific person by their email?**
Yes! Use the `get_person` tool with the Person ID. Your agent will respond with complete metadata for the record, including custom fields, account status, and activity history in seconds.

**Q: How do I find my Outseta API Key and Secret?**
Log in to your Outseta dashboard, navigate to **Settings** > **Integrations** > **API Keys**, and click 'Add API Key'. You will receive both an API Key and a Secret Key.

**Q: What is the subdomain?**
The subdomain is the unique prefix of your Outseta URL (e.g., if you log in at `my-startup.outseta.com`, the subdomain is `my-startup`).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outseta](https://vinkius.com/mcp/outseta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outseta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `outseta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outseta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outseta": {
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
