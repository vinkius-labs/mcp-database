# More Trees MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/more-trees)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Plant trees for every transaction and track your environmental impact with carbon offset certificates for sustainable businesses.

## Description
Connect your **More Trees** account to any AI agent and manage reforestation operations.

### What you can do

- **Project Management** — Browse reforestation projects and details
- **Tree Planting** — Submit planting orders with species and quantity
- **Transaction Tracking** — View planting history and status
- **Forest Exploration** — Browse forests with locations and tree counts
- **Impact Reports** — View CO2 offset and environmental metrics
- **Certificates** — Download digital planting certificates


## Available Tools
- **check_moretrees_status**: Verify API connectivity
- **get_account**: Get account info
- **get_certificate**: Get planting certificate
- **get_forest**: Get forest info
- **get_impact_report**: Get impact report
- **get_planting_status**: Get planting status
- **get_project**: Get project details
- **list_forests**: List all forests
- **list_projects**: List reforestation projects
- **list_transactions**: List planting transactions
- **plant_trees**: Plant trees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **More Trees** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plant 100 trees in the Amazon project."

**🤖 AI Agent:**
> Order placed! Transaction ID: txn_8291. 100 trees will be planted in the Amazon Reforestation Project. Species: Brazil Nut. Expected planting: next 30 days.

---

**👤 You:**
> "Show my environmental impact report."

**🤖 AI Agent:**
> Impact Report: 2,450 trees planted, 245 tons CO2 offset, 12.5 hectares reforested. This year: 890 trees, 89 tons CO2.

---

**👤 You:**
> "List all available forests."

**🤖 AI Agent:**
> 5 forests: Amazon Basin (Brazil, 12K trees), Borneo Rainforest (Indonesia, 8K), Kenya Highlands (3.5K), Portugal Atlantic (2K), Madagascar Coast (1.8K).


## ❓ FAQ

**Q: Can my AI plant trees?**
Yes! `plant_trees` submits a planting order. Specify the quantity, project, and species. You receive a transaction ID to track progress.

**Q: Can I track environmental impact?**
Yes. `get_impact_report` returns CO2 offset, total trees planted, and area reforested for your account.

**Q: Can I get planting certificates?**
Yes. `get_certificate` returns the digital certificate for any planting transaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/more-trees](https://vinkius.com/mcp/more-trees)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **More Trees** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `more-trees` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **More Trees** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "more-trees": {
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
