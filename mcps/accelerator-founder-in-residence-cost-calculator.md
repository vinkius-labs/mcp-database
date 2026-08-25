# Accelerator Founder-in-Residence Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-founder-in-residence-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the economic impact and investment requirements for hiring a Founder-in-Residence (EiR).

## Description
This MCP server provides specialized tools for venture studios to model the economics of their Founder-in-Residence (EiR) programs. It allows users to determine the total cash investment required for a residency, identify the break-even success rate needed to recover capital, and evaluate the structural efficiency of equity and salary balances. Use `get_total_investment` to calculate cumulative cash outlay, `calculate_breakeven_rate` to find the minimum required success probability, and `analyze_structure_efficiency` to assess the balance between EiR incentives and studio protection.


## Available Tools (3)
- **calculate_breakeven_rate**: Identifies the minimum likelihood of a successful venture exit needed to justify the EiR investment
- **analyze_structure_efficiency**: Evaluates whether the current equity and salary balance provides sufficient incentive for the EiR while protecting studio interests
- **get_total_investment**: Determines the total cash cost required to sustain an EiR through the residency period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Founder-in-Residence Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total investment for an EiR with a $10,000 monthly salary for 12 months?"

**🤖 AI Agent:**
> The total investment for an EiR with a $10,000 monthly salary over 12 months is $120,000.

---

**👤 You:**
> "If I spend $150,000 on an EiR and expect a $5,000,000 exit with a 20% studio share, what is the break-even success rate?"

**🤖 AI Agent:**
> The break-even success rate is 1.5%.

---

**👤 You:**
> "Analyze a structure with 15% equity for the EiR, $8,000 salary, 18 months residency, and 40% studio return share."

**🤖 AI Agent:**
> The structure provides a moderate incentive score and high studio protection, suggesting a balanced approach for capital preservation.


## ❓ FAQ

**Q: How do I calculate the total cost of an EiR?**
You can use the `get_total_investment` tool by providing the monthly salary and the number of months until the venture spins out.

**Q: What is the break-even success rate?**
It is the minimum probability of a successful exit required for the studio to recover its total investment based on its share of the exit value. Use `calculate_breakeven_rate` to find this value.

**Q: Can I evaluate if my equity split is fair?**
Yes, the `analyze_structure_efficiency` tool evaluates the balance between EiR incentives and studio protection based on salary, equity, and return shares.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-founder-in-residence-cost-calculator](https://vinkius.com/ai-agent-connect/accelerator-founder-in-residence-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Founder-in-Residence Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-founder-in-residence-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Founder-in-Residence Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-founder-in-residence-cost-calculator": {
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
