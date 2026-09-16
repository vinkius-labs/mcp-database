# Venture Vesting Acceleration MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-vesting-acceleration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the economic impact of equity acceleration during corporate exits.

## Description
This MCP server provides specialized financial modeling for venture-backed founders and investors. It calculates the economic impact of equity acceleration during changes of control. Use `calculate_acceleration_economics` to determine core financial metrics, `assess_retention_impact` to evaluate founder retention risks, `estimate_tax_impact` to model tax burdens, and `simulate_coc_scenarios` to compare single and double trigger costs.


## Available Tools (4)
- **assess_retention_impact**: 
- **calculate_acceleration_economics**: 
- **estimate_tax_impact**: 
- **simulate_coc_scenarios**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Vesting Acceleration** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the acceleration economics for 15% unvested shares with a single trigger at a $5.00 share price and 1,000,000 total shares."

**🤖 AI Agent:**
> The acceleration value is $750,000.00, with a total deal cost of $750,000.00 for the 150,000 unvested shares.

---

**👤 You:**
> "What is the retention impact for a founder with a $250,000 salary if the acceleration value is $1,000,000 using a double trigger?"

**🤖 AI Agent:**
> The retention score is high, as the double trigger structure incentivizes the founder to remain with the company to ensure the second trigger condition is met.

---

**👤 You:**
> "Estimate the tax impact for an acceleration value of $500,000 in a high-tax jurisdiction."

**🤖 AI Agent:**
> The estimated tax liability is $200,000.00, resulting in net proceeds of $300,000.00.


## ❓ FAQ

**Q: What is the difference between single and double trigger acceleration?**
Single trigger acceleration occurs immediately upon a Change of Control. Double trigger acceleration requires both a Change of Control and a subsequent termination of the founder.

**Q: How can I model the cost of an acquisition?**
You can use the `simulate_coc_scenarios` tool to model the total deal cost under different acquisition premiums and trigger types.

**Q: Does this tool account for tax implications?**
Yes, the `estimate_tax_impact` tool allows you to estimate the tax liability and net proceeds based on the acceleration value and jurisdiction tax levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-vesting-acceleration](https://vinkius.com/en/ai-agent-connect/venture-vesting-acceleration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Vesting Acceleration** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-vesting-acceleration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Vesting Acceleration** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-vesting-acceleration": {
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
