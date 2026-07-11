# Wedding Budget Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wedding-budget-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Intelligently allocate your wedding budget using industry-standard percentages and dynamic rebalancing.

## Description
The Wedding Budget Splitter helps you distribute your total wedding investment across key categories like Venue, Catering, and Photography. Use `standard_allocation` to get a baseline breakdown based on industry averages, or use `custom_allocation` to prioritize specific areas while the tool automatically rebalances the remaining funds. Additionally, use `estimate_hidden_costs` to account for often-overlooked expenses like taxes and service charges.


## Available Tools (3)
- **custom_allocation**: Calculate a custom wedding budget allocation
- **estimate_hidden_costs**: Estimate additional wedding expenses
- **standard_allocation**: Get a standard wedding budget allocation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Budget Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a total wedding budget of $30,000. What should my allocation look like?"

**🤖 AI Agent:**
> Based on standard industry averages for a $30,000 budget, you should allocate approximately $14,250 to Venue & Reception, $7,000 to Catering, $3,300 to Photography & Videography, and the remainder to other categories.

---

**👤 You:**
> "I want to spend 40% of my $20,000 budget on Catering. How does the rest of the budget distribute?"

**🤖 AI Agent:**
> With a 40% override for Catering in your $20,000 budget, the remaining $12,000 will be proportionally distributed among other categories like Venue & Reception and Photography based on their standard weights.

---

**👤 You:**
> "How much extra should I set aside for hidden fees in my catering budget of $8,000?"

**🤖 AI Agent:**
> For a $8,000 catering allocation, you can expect approximately $2,000 to $2,400 in additional hidden costs from taxes and service charges.


## ❓ FAQ

**Q: How does the standard allocation work?**
The `standard_allocation` tool uses industry-standard percentages to divide your total budget into categories like Venue, Catering, and Photography.

**Q: Can I prioritize certain wedding expenses?**
Yes, using `custom_allocation`, you can specify a percentage for specific categories. The tool will then rebalance the remaining budget across other categories to ensure your total stays at 100%.

**Q: Does it account for taxes and service charges?**
Yes, the `estimate_hidden_costs` tool calculates estimated additional expenses like taxes and gratuities specifically for Venue & Reception and Catering categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wedding-budget-splitter](https://vinkius.com/mcp/wedding-budget-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Budget Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-budget-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Budget Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-budget-splitter": {
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
