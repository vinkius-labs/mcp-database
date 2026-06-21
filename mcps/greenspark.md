# Greenspark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/greenspark)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Embed climate action into your product via Greenspark — plant trees, offset carbon, and track impact via AI.

## Description
Connect your **Greenspark** account to any AI agent and automate your business's environmental impact. Use natural language to trigger verified climate actions like planting trees or rescuing ocean plastic, and monitor your total sustainability goals in real-time.

### What you can do

- **Impact Orchestration** — Trigger new climate impacts programmatically by passing specific event data and quantities natively
- **Live Tracking** — Retrieve detailed impact records and summary reports to analyze your total environmental contribution flawlessly
- **Project Discovery** — List and explore the vetted environmental projects your contributions support globally
- **Emission Estimation** — Calculate the carbon footprint of transactions based on merchant categories to automate offsetting synchronously
- **Asset Management** — List and manage available impact badges and widgets to showcase your verified impact natively
- **Webhook Integration** — Configure and audit API webhooks to keep your internal systems synchronized with project updates flawlessly

### How it works

1. Subscribe to this server
2. Enter your Greenspark API Key (found in your Greenspark Dashboard under Settings > API)
3. Start automating your climate positive actions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sustainability Officers** — monitor real-time impact metrics and audit environmental projects via natural language
- **Product Managers** — embed climate rewards into user journeys and automate tree planting for specific user milestones
- **Operations Teams** — calculate and offset the carbon footprint of company operations and travel synchronously


## Available Tools
- **create_impact**: Trigger a new climate impact (e.g. plant a tree)
- **create_webhook**: Configure a new API webhook
- **estimate_footprint**: Calculate the carbon footprint of a transaction
- **get_impact_summary**: Get total aggregated impact data for the account
- **get_impact**: Get details for a specific impact record
- **get_project**: Get details for a specific environmental project
- **get_subscription**: Get details of the account Greenspark subscription
- **list_badges**: List available impact badges and widgets
- **list_impact_types**: List available types of climate impact
- **list_impacts**: List historical climate impacts generated
- **list_projects**: List environmental projects supported by Greenspark
- **list_webhooks**: List configured API webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Greenspark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my total climate impact summary"

**🤖 AI Agent:**
> Retrieving your impact summary... To date, your business has: 1. Planted 1,240 trees. 2. Offset 45,000 kg of CO2. 3. Rescued 12,500 plastic bottles. Would you like to see the specific projects these impacts supported?

---

**👤 You:**
> "Plant 10 trees for our latest customer sale"

**🤖 AI Agent:**
> Processing climate action... Success! I've triggered the planting of 10 trees via the Eden Reforestation Projects. Your total tree count is now 1,250.

---

**👤 You:**
> "Estimate the carbon footprint of a $50 flight purchase"

**🤖 AI Agent:**
> Calculating footprint... For a $50 transaction in the 'Airlines' category, the estimated impact is 125 kg of CO2e. Would you like to offset this amount now?


## ❓ FAQ

**Q: Can my agent trigger a climate impact like planting a tree through chat?**
Yes. Use the 'create_impact' tool. By passing the impact type (e.g., 'tree') and the quantity, the agent can programmatically trigger verified climate actions natively through Greenspark's API.

**Q: How do I check my total accumulated impact via chat?**
You can use the 'get_impact_summary' tool. Your agent will fetch the total count of trees planted, kg of CO2 offset, and plastic bottles rescued, providing a real-time overview of your sustainability goals flawlessly.

**Q: Can I calculate the carbon footprint of a transaction through the agent?**
Absolutely. Use the 'estimate_footprint' tool. Provide the transaction amount and merchant category, and your agent will return the estimated CO2e impact using Greenspark's estimation engines synchronously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/greenspark](https://vinkius.com/mcp/greenspark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Greenspark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `greenspark` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Greenspark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "greenspark": {
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
