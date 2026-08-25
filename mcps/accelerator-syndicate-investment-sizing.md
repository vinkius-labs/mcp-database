# Accelerator Syndicate Investment Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-syndicate-investment-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal capital allocation and strategic positioning for accelerator-led investment syndicates.

## Description
This MCP server provides specialized investment intelligence for accelerator-led syndicates. It helps fund managers determine optimal capital allocation by analyzing the interplay between lead investor footprints and target participation. Use `calculate_allocation_strategy` to determine recommended investment amounts and strategic positioning, `analyze_syndicate_headroom` to verify if target allocations are mathematically feasible, and `evaluate_relationship_value` to adjust sizing based on strategic importance and follow-on capacity constraints.


## Available Tools (3)
- **analyze_syndicate_headroom**: Analyzes if the accelerator's target is mathematically feasible within the current round structure
- **calculate_allocation_strategy**: Calculates optimal capital allocation and strategic positioning for accelerator-led investment syndicates
- **evaluate_relationship_value**: Evaluates how much the strategic importance of the deal should influence the sizing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Syndicate Investment Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the allocation strategy for a $5,000,000 round where the lead takes 40%, our target is 10%, and we have co-investment rights with a relationship score of 8."

**🤖 AI Agent:**
> The recommended allocation is $500,000. Given the high relationship score and co-investment rights, the strategy is a Strategic Follow-on to preserve capacity for future rounds.

---

**👤 You:**
> "Is a 25% target allocation feasible for a $2,000,000 round if the lead investor is taking 80%?"

**🤖 AI Agent:**
> No, the target allocation is impossible. The available capacity after the lead investor's share is only 20%.

---

**👤 You:**
> "Adjust a $200,000 base allocation for a deal with a relationship score of 9, but I have limited follow-on capacity."

**🤖 AI Agent:**
> The adjusted allocation is $150,000. Due to the follow-on capacity constraint, the allocation was reduced to prioritize future participation.


## ❓ FAQ

**Q: How does the tool handle lead investor constraints?**
The tool uses `calculate_allocation_strategy` to ensure the recommended allocation respects the lead investor's footprint. If the target allocation exceeds the available space, the tool adjusts the recommendation downwards.

**Q: Can I check if my target allocation is possible?**
Yes, you can use `analyze_syndicate_headroom` to check if your desired share is mathematically feasible given the lead investor's percentage.

**Q: How is strategic importance factored into the sizing?**
The `evaluate_relationship_value` tool allows you to adjust the base allocation by considering a relationship value score and any current follow-on capacity constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-syndicate-investment-sizing](https://vinkius.com/ai-agent-connect/accelerator-syndicate-investment-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Syndicate Investment Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-syndicate-investment-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Syndicate Investment Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-syndicate-investment-sizing": {
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
