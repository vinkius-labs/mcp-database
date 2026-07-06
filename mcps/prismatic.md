# Prismatic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prismatic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Prismatic integration platform — list customers, create instances, deploy integrations, and fetch execution logs via AI.

## Description
Connect your **Prismatic** environment to any AI agent to streamline your embedded iPaaS workflows. This server allows you to manage the entire lifecycle of your B2B integrations through natural language.

### What you can do

- **Customer Management** — List all customers and create new customer records with external IDs for seamless mapping.
- **Instance Lifecycle** — Create new integration instances for specific customers and deploy them to make configuration changes live.
- **Observability & Debugging** — Fetch detailed execution logs between specific timestamps to monitor integration health and troubleshoot issues.
- **Advanced GraphQL Access** — Execute custom GraphQL queries or mutations to access any part of the Prismatic schema, including components, actions, and user configurations.

### How it works

1. Subscribe to this server
2. Enter your Prismatic API Token
3. Start managing your integrations, customers, and deployments directly from your favorite MCP client.

### Who is this for?

- **DevOps & Integration Engineers** — Deploy instances and check logs without leaving the terminal or IDE.
- **Product Managers** — Quickly list customers and verify which integrations are active for specific accounts.
- **Support Teams** — Investigate execution logs to resolve customer issues faster using AI-assisted log analysis.


## Available Tools (6)
- **fetch_logs**: Fetch execution logs
- **run_graphql**: Execute a custom GraphQL query or mutation
- **create_customer**: Create a new Prismatic customer
- **create_instance**: Create a new integration instance
- **list_customers**: Fetch all Prismatic customers
- **deploy_instance**: Deploy an integration instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prismatic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers currently configured in Prismatic."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 3 customers: 'Acme Corp' (ID: cust_123), 'Globex' (ID: cust_456), and 'Soylent Corp' (ID: cust_789).

---

**👤 You:**
> "Deploy the instance with ID inst_98765."

**🤖 AI Agent:**
> Deployment triggered for instance inst_98765. The configuration changes are now being applied to the runtime environment.

---

**👤 You:**
> "Fetch logs from the last 10 minutes (between 2023-10-27T10:00:00Z and 2023-10-27T10:10:00Z)."

**🤖 AI Agent:**
> I've fetched the logs for that period. I found 12 events, including a 'Webhook Received' success and one 'Execution Error' related to a timeout in the Slack component.


## ❓ FAQ

**Q: Can I execute custom GraphQL queries if a specific tool isn't available?**
Yes! Use the `run_graphql` tool to execute any valid Prismatic GraphQL query or mutation. This gives you full access to the schema, including actions, components, and user data.

**Q: How do I make sure my integration changes are actually live?**
After creating or updating an instance, you must use the `deploy_instance` tool with the specific Instance ID. This triggers the deployment process required for changes to take effect.

**Q: Is it possible to filter logs by a specific time range?**
Yes, the `fetch_logs` tool requires `timestampGte` and `timestampLte` parameters in DateTime format, allowing you to pinpoint exactly when an event occurred.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prismatic](https://vinkius.com/mcp/prismatic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prismatic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prismatic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prismatic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prismatic": {
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
