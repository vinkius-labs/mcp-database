# Replacement Purchase Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/replacement-purchase-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Evaluate product replacements by matching failed item needs against inventory using budget and warranty constraints.

## Description
This MCP server helps users find the perfect replacement for a failed item. It analyzes failed item needs and prioritized replacement specifications against available inventory. Use `get_shortlist` to find products within budget, `validate_spec_compatibility` to ensure technical fit, `compare_warranty_options` to check coverage, and `get_purchase_checklist` for a final verification before buying.


## Available Tools (4)
- **compare_warranty_options**: Evaluates the warranty strength of a specific product against the user's stated preference
- **get_purchase_checklist**: Provides a final verification checklist for a single selected product
- **get_shortlist**: Generates a curated list of products that most closely match the failed item's needs while staying within budget
- **validate_spec_compatibility**: Checks if a specific product's attributes can accommodate the requirements of the failed item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Replacement Purchase Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a replacement for my broken vacuum within $200 that has high suction power."

**🤖 AI Agent:**
> I have found two suitable vacuum cleaners within your $200 budget that meet the suction power requirements.

---

**👤 You:**
> "Is this specific laptop compatible with my old charger's voltage requirements?"

**🤖 AI Agent:**
> No, the voltage requirements of the new laptop do not match the specifications of your existing charger.

---

**👤 You:**
> "Check if the warranty for the Pro-Series Drill meets my preference for 3-year coverage."

**🤖 AI Agent:**
> Yes, the Pro-Series Drill comes with a 3-year manufacturer warranty, which meets your preference.


## ❓ FAQ

**Q: How does the tool select replacement products?**
The `get_shortlist` tool selects products by matching their specifications to the failed item's needs while strictly adhering to your budget constraint.

**Q: Can I verify if a product fits my technical requirements?**
Yes, you can use `validate_spec_compatibility` to check if a candidate product's attributes meet the required physical or technical dimensions.

**Q: How do I ensure I don't overspend?**
The system enforces budget constraints during the `get_shortlist` process and provides a final `get_purchase_checklist` to verify the price is within your limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/replacement-purchase-brief](https://vinkius.com/en/ai-agent-connect/replacement-purchase-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Replacement Purchase Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `replacement-purchase-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Replacement Purchase Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "replacement-purchase-brief": {
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
