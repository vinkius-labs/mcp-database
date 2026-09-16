# Venture Scout Program Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-scout-program-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze the ROI, sustainability, and distribution of venture capital scout programs.

## Description
This MCP server provides a financial modeling engine to evaluate the efficiency and sustainability of venture capital scout programs. It connects AI agents to specialized tools like `scout_program_roi` for calculating program ROI, `carry_sustainability_check` to ensure the carry pool covers operational costs, `scout_performance_analysis` to factor in scout quality, and `pool_distribution_planner` to model carry distribution among scouts. It is designed to help fund managers optimize their scout networks by analyzing the relationship between program overhead and deal sourcing performance.


## Available Tools (4)
- **carry_sustainability_check**: Determines if the allocated carry pool is sufficient to cover the program's operational costs
- **pool_distribution_planner**: Models how the carry pool would be distributed among scouts based on their individual deal attribution
- **scout_performance_analysis**: Evaluates the efficiency of the scout network by factoring in scout quality
- **scout_program_roi**: Calculates the return on investment for the entire scout program


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Scout Program Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ROI for a program with 10 scouts, 5% carry allocation, 20 deals sourced, 20% carry rate, $50,000 cost, and $10,000 projected carry per deal?"

**🤖 AI Agent:**
> The total projected carry is $200,000, and the program ROI is 4.0.

---

**👤 You:**
> "Is a program sustainable if the carry pool is $100,000 and the program cost is $120,000?"

**🤖 AI Agent:**
> No, the program is not sustainable as the carry pool does not cover the total program cost.

---

**👤 You:**
> "Calculate the effective deal count for 5 scouts, 10 deals sourced, and an average scout quality of 1.5."

**🤖 AI Agent:**
> The effective deal count is 15.


## ❓ FAQ

**Q: How can I calculate the ROI of my scout program?**
You can use the `scout_program_roi` tool, providing the number of scouts, carry allocation, deals sourced, carry rate, program cost, and projected carry per deal.

**Q: How do I check if my scout carry pool is sustainable?**
Use the `carry_sustainability_check` tool to compare the allocated carry pool against the total program cost.

**Q: Can I model how carry is distributed among individual scouts?**
Yes, the `pool_distribution_planner` tool allows you to model the distribution of the carry pool based on individual deal attribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-scout-program-economics](https://vinkius.com/en/ai-agent-connect/venture-scout-program-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Scout Program Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-scout-program-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Scout Program Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-scout-program-economics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
