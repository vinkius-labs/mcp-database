# Streaming Plan Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/streaming-plan-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare streaming service bundles by price, content, and user capacity.

## Description
This MCP server provides a specialized comparison engine for streaming service bundles. It allows AI agents to evaluate different subscription packages based on cost-efficiency, content availability, and user experience metrics. Users can find the best value by comparing monthly versus annual costs, filtering by desired services, and ranking bundles by metrics like lowest price or most services. Use `get_available_bundles` to see what is available in a region, `filter_bundles_by_requirements` to find specific content matches, and `evaluate_value_proposition` to rank the best deals.


## Available Tools (4)
- **evaluate_value_proposition**: Ranks a selection of bundles based on a "value score" relative to user needs
- **filter_bundles_by_requirements**: Finds bundles that match a user's specific content and user-capacity needs
- **get_available_bundles**: Retrieves a list of all available streaming bundles currently in the catalog
- **compare_bundle_pricing**: Calculates and compares the long-term financial impact of different bundles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Streaming Plan Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What streaming bundles are available in the USA?"

**🤖 AI Agent:**
> In the USA, available bundles include the 'Basic Duo' at $12.99/month and the 'Premium Family Pack' at $24.99/month.

---

**👤 You:**
> "Find me a bundle in Europe that includes Netflix and Disney+."

**🤖 AI Agent:**
> The 'EuroStream Max' bundle is a match, as it includes both Netflix and Disney+ for €15.99 per month.

---

**👤 You:**
> "Which bundle is the cheapest for 4 users?"

**🤖 AI Agent:**
> The 'Family Saver' bundle is the most cost-effective option for 4 users, priced at $18.00 per month.


## ❓ FAQ

**Q: How can I find bundles that include specific services?**
You can use the `filter_bundles_by_requirements` tool and specify the platforms you want in the `desiredServices` parameter.

**Q: Does this tool account for annual discounts?**
Yes, the `compare_bundle_pricing` tool allows you to set `isAnnual` to true to calculate the total cost and effective monthly rate for a 12-month commitment.

**Q: Can I filter by the number of users allowed in a plan?**
Yes, you can use `filter_bundles_by_requirements` with the `minUsers` parameter to find plans that support your household size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/streaming-plan-comparator](https://vinkius.com/en/ai-agent-connect/streaming-plan-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Streaming Plan Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `streaming-plan-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Streaming Plan Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "streaming-plan-comparator": {
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
