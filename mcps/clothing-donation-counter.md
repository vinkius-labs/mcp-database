# Clothing Donation Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/clothing-donation-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Track and analyze donated garment counts and quality distributions.

## Description
This MCP server provides tools to manage and analyze clothing donation data. Use `get_donation_tally` to see total counts by category, `get_condition_distribution` to check item quality, `get_impact_tier` to classify donation scale, and `get_category_summary` for a full list of garment types.


## Available Tools (4)
- **get_category_summary**: Detailed list of categories
- **get_condition_distribution**: Distribution of quality grades
- **get_donation_tally**: Provides a summary of total garments
- **get_impact_tier**: Determines scale of donation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clothing Donation Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many tops have been donated so far?"

**🤖 AI Agent:**
> There have been 45 tops donated so far.

---

**👤 You:**
> "What is the quality distribution of the received items?"

**🤖 AI Agent:**
> The distribution is: New: 10, Excellent: 25, Good: 15, Fair: 5.

---

**👤 You:**
> "Is a donation of 500 items considered an Enterprise tier?"

**🤖 AI Agent:**
> Yes, a donation of 500 items falls under the Enterprise impact tier.


## ❓ FAQ

**Q: How do I see the total number of donated items?**
You can use the `get_donation_tally` tool to get a summary of total garments received.

**Q: Can I filter counts by a specific type of clothing?**
Yes, the `get_donation_tally` tool accepts a category filter to narrow down the results.

**Q: How is the donation impact scale determined?**
The `get_impact_tier` tool determines if a donation is Individual, Community, or Enterprise based on the item count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/clothing-donation-counter](https://vinkius.com/en/ai-agent-connect/clothing-donation-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clothing Donation Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clothing-donation-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clothing Donation Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clothing-donation-counter": {
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
