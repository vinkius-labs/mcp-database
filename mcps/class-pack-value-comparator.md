# Class Pack Value Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/class-pack-value-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluates the true cost of fitness pricing models by factoring in attendance probability and travel costs.

## Description
This MCP server provides a specialized financial engine to determine the most economical way to attend fitness classes. It compares drop-in fees, pre-paid class packs, and monthly memberships by calculating the 'effective cost' per session. Unlike simple division, it uses `get_class_pack_value` to account for the likelihood of actually using all credits before they expire, and `compare_all_models` to provide a side-by-side comparison of all options including travel expenses.


## Available Tools (4)
- **compare_all_models**: Provides a side-by-side comparison of the three pricing models
- **get_class_pack_value**: Calculates the true cost of a pre-paid bundle by adjusting for the likelihood of actual attendance and expiration
- **get_drop_in_cost**: Calculates the total cost of attending a specific number of classes using only single-session payments
- **get_membership_value**: Calculates the cost of a recurring monthly membership model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Class Pack Value Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to attend 10 classes. Drop-in is $15, a 10-pack is $120 with an 80% chance I use them all, and a membership is $50/month plus $5 per class. Travel is $3 per visit. Which is cheapest?"

**🤖 AI Agent:**
> The most economical choice is the class pack, with a total expected cost of $144.00.

---

**👤 You:**
> "Calculate the effective cost of a 20-class pack that costs $200 if I only have a 70% chance of using every credit and travel is $5 per visit."

**🤖 AI Agent:**
> The effective cost per class is $33.33, with a total expected cost of $210.00 for 14 expected visits.

---

**👤 You:**
> "What is the total cost for 5 drop-in sessions if each session is $20 and travel is $4?"

**🤖 AI Agent:**
> The total cost for 5 drop-in sessions is $120.00.


## ❓ FAQ

**Q: How does this tool account for unused class credits?**
It uses an attendance probability coefficient. By using `get_class_pack_value`, the tool calculates the effective cost based on how many classes you are actually likely to attend, rather than the total number of credits purchased.

**Q: Does it include travel expenses in the comparison?**
Yes. All models, including drop-in and membership, factor in the `travelCostPerVisit` to ensure you see the true total expenditure for each session.

**Q: Can I compare all my options at once?**
Yes, you can use `compare_all_models` to receive a side-by-side breakdown of drop-in, pack, and membership costs to find the cheapest option.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/class-pack-value-comparator](https://vinkius.com/en/ai-agent-connect/class-pack-value-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Class Pack Value Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `class-pack-value-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Class Pack Value Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "class-pack-value-comparator": {
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
