# Valid Outfit Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/valid-outfit-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate and sample valid clothing combinations based on formality consistency rules.

## Description
The Valid Outfit Generator MCP server connects AI agents to a rule-based engine that calculates possible clothing combinations. It enforces 'Formality Consistency', ensuring that items tagged as 'formal' are never mixed with those tagged as '..'casual'. Use `count_valid_outfits` to find the total number of valid ensembles, `get_outfit_samples` to preview specific combinations, or `verify_outfit_consistency` to check if a pre-selected group of items adheres to the rules. This tool is ideal for fashion styling agents and wardrobe management workflows.


## Available Tools (3)
- **count_valid_outfits**: Calculates the total number of possible clothing combinations that satisfy the formality consistency rule
- **get_outfit_samples**: Retrieves a limited list of valid clothing combinations for previewing
- **verify_outfit_consistency**: Validates whether a specific, pre-selected group of items adheres to the formality rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Valid Outfit Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many valid outfits can I make with these tops: [{'id': 't1', 'tags': ['formal']}], bottoms: [{'id': 'b1', 'tags': ['casual']}], and shoes: [{'id': 's1', 'tags': ['casual']}]?"

**🤖 AI Agent:**
> 0 valid outfits found. The combination is invalid because it mixes a 'formal' top with 'casual' bottoms and shoes.

---

**👤 You:**
> "Check if this outfit is consistent: [{'id': 't1', 'tags': ['casual']}, {'id': 'b1', 'tags': ['casual']}]"

**🤖 AI Agent:**
> true

---

**👤 You:**
> "Give me 2 samples from these items: tops: [{'id': 't1', 'tags': ['casual']}], bottoms: [{'id': 'b1', 'tags': ['casual']}], shoes: [{'id': 's1', 'tags': ['casual']}]"

**🤖 AI Agent:**
> [["t1", "b1", "s1"]]


## ❓ FAQ

**Q: What is Formality Consistency?**
It is a rule that prevents mixing items with 'formal' and 'casual' tags in the same outfit.

**Q: Which categories are required for an outfit?**
Every valid outfit must include at least one top, one bottom, and one pair of shoes.

**Q: Can I include layers in my calculation?**
Yes, you can optionally provide a 'layers' array. Any items added must also follow the formality consistency rule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/valid-outfit-generator](https://vinkius.com/mcp/valid-outfit-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Valid Outfit Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `valid-outfit-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Valid Outfit Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "valid-outfit-generator": {
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
