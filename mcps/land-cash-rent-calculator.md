# Land Cash Rent Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/land-cash-rent-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine equitable cash rent using crop-share equivalency, margin analysis, and yield probability.

## Description
This MCP server provides precision tools for landowners and tenants to negotiate fair cash rent agreements. It reconciles economic interests by calculating the Cash Rent Equivalent (CRE) to match crop-share models, analyzing net margins for both parties, and generating rent ranges based on historical yield probability distributions. Users can also access USDA-aligned market benchmarks to ensure local competitiveness.


## Available Tools (4)
- **calculate_party_margins**: Answers how much profit both the landlord and the tenant will actually pocket at a specific rent level
- **fetch_market_benchmarks**: Answers what the current local market rates are according to official data
- **generate_rent_probability_range**: Answers what the "safe" rent range is given the uncertainty of crop yields
- **get_rent_equivalency**: Answers how much cash rent is needed to match the value of a crop-share agreement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Land Cash Rent Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cash rent equivalent for a crop with $500,000 revenue, a 25% landlord share, and $50,000 in non-land costs?"

**🤖 AI Agent:**
> The cash rent equivalent is $175,000.

---

**👤 You:**
> "Calculate the landlord and tenant margins for a $10,000 rent, $50,000 revenue, $20,000 non-land costs, and $2,000 landlord expenses."

**🤖 AI Agent:**
> The landlord net return is $8,000 and the tenant net return is $20,000.

---

**👤 You:**
> "What are the market benchmarks for corn in region code 12345?"

**🤖 AI Agent:**
> The average cash rent for corn in region 12345 is $250 per acre, with the 50th percentile at $245.


## ❓ FAQ

**Q: How do I calculate the cash rent equivalent?**
Use the `get_rent_equivalency` tool. Provide the expected crop revenue, the landowner's share percentage, and the non-land costs to find the fixed cash amount that matches a crop-share arrangement.

**Q: Can I see the profit margins for both parties?**
Yes, the `calculate_party_margins` tool calculates the net return for both the landlord and the tenant based on the proposed rent and operating costs.

**Q: How does the tool handle yield uncertainty?**
The `generate_rent_probability_range` tool uses historical yield data to simulate revenue scenarios, providing a rent range and a probability distribution of profitable rent levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/land-cash-rent-calculator](https://vinkius.com/ai-agent-connect/land-cash-rent-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Land Cash Rent Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `land-cash-rent-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Land Cash Rent Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "land-cash-rent-calculator": {
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
