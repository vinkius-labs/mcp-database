# Accelerator Carry Distribution MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-carry-distribution)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate venture capital waterfall distributions, GP catch-ups, and clawback scenarios.

## Description
This MCP server provides precise financial modeling for venture capital fund distributions. It implements a standard four-tier waterfall model to determine how exit proceeds are split between Limited Partners (LP) and the General Partner (GP). Use `calculate_waterfall_distribution` to determine exact dollar amounts for LPs and GP based on capital, hurdle rates, and carried interest. You can also use `simulate_clawback_scenario` to evaluate potential GP liabilities if fund performance changes, or `analyze_irr_sensitivity` to see how different hurdle rates impact the GP's catch-up phase. It is designed for fund managers and analysts needing accurate distribution modeling.


## Available Tools (3)
- **analyze_irr_sensitivity**: Provides a comparison of how different hurdle rates affect the GP's ability to enter the catch-up phase
- **calculate_waterfall_distribution**: Determines the exact dollar amounts distributed to LPs and the GP based on the fund's performance and agreement terms
- **simulate_clawback_scenario**: Evaluates the potential impact on the GP if the fund's performance drops after a large exit, requiring the return of carried interest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Carry Distribution** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the waterfall for a fund with $50M gross proceeds, $40M LP capital, 20% carried interest, and an 8% hurdle rate."

**🤖 AI Agent:**
> The distribution results in $43,200,000 for LPs and $6,800,000 for the GP, with a total profit of $10,000,000.

---

**👤 You:**
> "What happens if the GP has already received $2M in carry but the final fund profit is only $8M with a 20% carry agreement?"

**🤖 AI Agent:**
> The GP is required to return $400,000 to the LPs to satisfy the 20% carried interest agreement on the $8M profit.

---

**👤 You:**
> "Compare how hurdle rates of 5%, 8%, and 10% affect the GP carry for a fund with $100M proceeds and $80M LP capital."

**🤖 AI Agent:**
> At a 5% hurdle, the GP carry is $4,000,000; at 8%, it is $3,600,000; and at 10%, it is $3,200,000.


## ❓ FAQ

**Q: What is a waterfall distribution?**
A waterfall distribution is a method used in venture capital to distribute fund proceeds. It follows specific tiers: returning capital to LPs, providing a preferred return (hurdle), a GP catch-up, and finally the carried interest split.

**Q: How does the GP catch-up work?**
The GP catch-up is a tier that allows the General Partner to receive a portion of the profits so that their total share of the distributed profits matches the agreed carried interest percentage after the LPs have received their preferred return.

**Q: Can I simulate a clawback?**
Yes, you can use the `simulate_clawback_scenario` tool to calculate how much carry a GP might need to return to LPs if the total fund profit falls below the level required to justify the carry already distributed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-carry-distribution](https://vinkius.com/ai-agent-connect/accelerator-carry-distribution)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Carry Distribution** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-carry-distribution` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Carry Distribution** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-carry-distribution": {
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
