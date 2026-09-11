# Finding and Development Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/finding-and-development-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate finding and development (F&D) costs per BOE for oil and gas reserves.

## Description
This MCP server provides specialized tools to calculate critical oil and gas industry metrics. It allows AI agents to determine the efficiency of capital deployment by calculating finding cost per BOE, development cost per BOE, and total F&D expenditure. Using tools like `get_fd_summary_report`, agents can generate comprehensive reports that account for exploration capital, development capital, and reserve additions to evaluate resource acquisition efficiency.


## Available Tools (4)
- **get_development_cost_per_boe**: Calculates the efficiency of development activities
- **get_fd_summary_report**: Provides a comprehensive breakdown of all F&D metrics for a given period
- **get_finding_cost_per_boe**: Calculates the efficiency of exploration activities
- **get_total_fd_cost**: Calculates the total capital expenditure for finding and development


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finding and Development Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total F&D cost if exploration capital is 500M and development capital is 300M?"

**🤖 AI Agent:**
> The total F&D cost is 800,000,000.

---

**👤 You:**
> "Calculate the finding cost per BOE for 100M exploration capital and 5M BOE reserve additions."

**🤖 AI Agent:**
> The finding cost per BOE is 20.

---

**👤 You:**
> "Provide a summary report for 200M exploration, 150M development, and 10M BOE reserves."

**🤖 AI Agent:**
> Total F&D cost is 350,000,000, finding cost per BOE is 20, development cost per BOE is 15, and total reserve additions are 10,000,000 BOE.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It calculates finding and development (F&D) costs per barrel of oil equivalent (BOE) to help evaluate capital efficiency in energy projects.

**Q: How do I get a full breakdown of my costs?**
You can use the `get_fd_summary_report` tool to receive a complete summary including total F&D cost, finding cost per BOE, and development cost per BOE.

**Q: Can I calculate development costs separately?**
Yes, the `get_development_cost_per_boe` tool allows you to isolate development efficiency specifically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/finding-and-development-cost-calculator](https://vinkius.com/ai-agent-connect/finding-and-development-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Finding and Development Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `finding-and-development-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Finding and Development Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "finding-and-development-cost-calculator": {
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
