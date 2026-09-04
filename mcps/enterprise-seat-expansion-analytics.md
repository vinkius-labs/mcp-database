# Enterprise Seat Expansion Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-seat-expansion-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enterprise](../categories/enterprise.md)

Calculate seat growth, adoption trends, and expansion opportunities.

## Description
This MCP server provides a specialized analytics engine for enterprise account growth. It allows AI agents to calculate seat expansion rates, track seat adoption velocity, and identify high-potential expansion opportunities. Using tools like `calculate_expansion_metrics`, `analyze_account_trend`, `identify_expansion_opportunities`, and `evaluate_adoption_depth`, agents can monitor how deeply a product is embedded within an organization by analyzing department adoption and use case spread.


## Available Tools (4)
- **analyze_account_trend**: ]

Determine the direction and velocity of seat adoption
- **calculate_expansion_metrics**: Calculate high-level growth performance metrics over a specific period
- **evaluate_adoption_depth**: Assess product embedding via departmental and use-case spread
- **identify_expansion_opportunities**: Identify accounts primed for additional seat purchases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Seat Expansion Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the expansion rate for an account that went from 50 to 75 seats in 6 months?"

**🤖 AI Agent:**
> The expansion rate for this account is 50%.

---

**👤 You:**
> "Is this account showing an increasing trend in seat adoption? History: [{"seatCount": 10, "monthIndex": 1}, {"seatCount": 25, "monthIndex": 2}]"

**🤖 AI Agent:**
> Yes, the trend is increasing with an average monthly velocity of 15 seats.

---

**👤 You:**
> "Identify expansion opportunities for an account with 100 seats, 95% utilization, and met expansion triggers."

**🤖 AI Agent:**
> The opportunity score is high, and the recommendation is to initiate an expansion conversation immediately due to high utilization.


## ❓ FAQ

**Q: How do I calculate the expansion rate?**
You can use the `calculate_expansion_metrics` tool by providing the initial seats, current seats, and the time period in months.

**Q: Can I identify accounts ready for more seats?**
Yes, the `identify_expansion_opportunities` tool flags accounts based on utilization rates and expansion triggers.

**Q: How is adoption depth measured?**
The `evaluate_adoption_depth` tool assesses embedding by looking at the number of departments and functional use cases active in the account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-seat-expansion-analytics](https://vinkius.com/ai-agent-connect/enterprise-seat-expansion-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Seat Expansion Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-seat-expansion-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Seat Expansion Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-seat-expansion-analytics": {
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
