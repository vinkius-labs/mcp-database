# Make.com Webhook Trigger MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/makecom-webhook-trigger)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

This MCP does exactly one thing: it sends JSON payloads to Make.com Webhooks. That's its only function. Incredible for connecting AI agents to thousands of visual automation workflows instantly.

## Description
We refused to build thousands of individual MCP integrations for every SaaS app in the world. Instead, this MCP server provides a universal, zero-trust bridge to Make.com (formerly Integromat): **just triggering a Custom Webhook.**

Your AI agent gains the immediate, zero-friction ability to kick off complex workflows—like generating contracts, issuing invoices, or adding contacts to CRMs—by simply dumping a structured JSON payload into a Make.com scenario.

### The Superpowers

- **The Ultimate Joker Card:** Why code a custom API integration when you can just build a scenario in Make? The agent sends the data, and Make does the visual routing to over 5,000+ apps.
- **Zero-Bloat Integration:** No massive SDKs. It uses a direct `POST` fetch to your specific Make Custom Webhook URL. You just provide the URL and the AI provides the JSON.
- **Absolute Containment:** Because this is strictly a sending tool (Push only), the agent cannot read your Make.com account, cannot edit your scenarios, and cannot access other webhooks. It is a secure, one-way trigger.


## Available Tools
- **trigger_make_webhook**: com scenario. Provide the data you want to send in the "payloadJson" parameter as a valid JSON string. The Make scenario will receive this data and process it.

Send a JSON payload to a Make.com (Integromat) Custom Webhook to trigger an automation scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Make.com Webhook Trigger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger the Make webhook with a JSON payload containing the customer's name and email to start the onboarding flow."

**🤖 AI Agent:**
> I've successfully triggered the Make.com webhook with the requested payload.


## ❓ FAQ

**Q: Can the agent receive responses back from Make.com with this?**
No. Make Webhooks respond immediately with 'Accepted'. The agent cannot wait for the scenario to finish executing or retrieve data from the final step of the Make scenario. This is strictly a 'fire and forget' trigger.

**Q: Do I need a paid Make.com account?**
No. You can use Custom Webhooks on the free tier of Make.com. You just need to create a new scenario starting with the 'Custom Webhook' module.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makecom-webhook-trigger](https://vinkius.com/mcp/makecom-webhook-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Make.com Webhook Trigger** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `makecom-webhook-trigger` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Make.com Webhook Trigger** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "makecom-webhook-trigger": {
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
