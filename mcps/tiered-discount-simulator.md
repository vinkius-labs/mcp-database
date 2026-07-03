# Tiered Discount Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tiered-discount-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the most cost-effective way to reach higher discount tiers by adding filler items.

## Description
The Tiered Discount Simulator is a logic engine designed to help shoppers maximize their savings. By analyzing current cart totals against available spending thresholds, it identifies if adding low-cost 'filler' items will trigger a higher discount percentage that outweighs the cost of the extra item. Using tools like `check_discount`, `calculate_upsell_impact`, and `find_optimal_strategy`, users can instantly see if their net cost drops by strategically increasing their basket value. This MCP server connects AI agents to complex threshold-based discounting logic, providing clear, actionable recommendations for optimal shopping efficiency.


## Available Tools (3)
- **check_discount**: Check the current discount applied to a cart total
- **calculate_upsell_impact**: Calculate the financial impact of adding a filler item
- **find_optimal_strategy**: Find the most cost-effective filler amount to reach a higher tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tiered Discount Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have $150 in my cart. My tiers are: $100 for 10% and $200 for 20%. Should I add a $50 item?"

**🤖 AI Agent:**
> Adding a $50 item to reach the $200 tier will result in a net cost of $160. Since your current net cost is $135, this is not beneficial.

---

**👤 You:**
> "Find the best strategy for a $180 cart with tiers: $100 (10%) and $200 (20%)."

**🤖 AI Agent:**
> Add a $20 item to save $4. Your net cost drops by $0.

---

**👤 You:**
> "Check my current discount for a $120 cart with a 10% tier at $100."

**🤖 AI Agent:**
> Your current applied discount is 10%, resulting in savings of $12.00.


## ❓ FAQ

**Q: How does the simulator determine if an upsell is beneficial?**
The engine compares your current net cost to the new net cost after adding a filler item. If the higher discount percentage reduces the total amount paid (including the filler) below your original spending level, it is flagged as beneficial.

**Q: What tools are available in this MCP server?**
The server provides `check_discount` to see your current savings, `calculate_upsell_impact` to test specific filler amounts, and `find_optimal_strategy` to automatically find the best possible threshold to reach.

**Q: Can I use my own discount rules?**
Yes. You can pass your specific spending thresholds and corresponding discount percentages as a JSON array to any of the tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tiered-discount-simulator](https://vinkius.com/mcp/tiered-discount-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tiered Discount Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tiered-discount-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tiered Discount Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tiered-discount-simulator": {
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
