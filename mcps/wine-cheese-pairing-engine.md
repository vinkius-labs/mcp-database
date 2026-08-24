# Wine & Cheese Pairing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-cheese-pairing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culinary](../categories/culinary.md)

A deterministic engine for calculating precise wine and cheese pairing scores.

## Description
This MCP server provides a scientific approach to culinary pairings. By analyzing chemical interactions like fat-tannin buffering and acidity-cutting, it calculates a compatibility score between specific wine and cheese profiles. Use `analyze_pairing` to get a detailed score and reasoning, `get_alternative_pairings` to discover new wine options for a cheese, or `validate_profiles` to ensure your data follows the engine's strict sensory constraints.


## Available Tools (3)
- **analyze_pairing**: 
- **get_alternative_pairings**: 
- **validate_profiles**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine & Cheese Pairing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the pairing score for a full-bodied Cabernet Sauvignon from Napa with a high-fat aged Cheddar?"

**🤖 AI Agent:**
> Score: 85. Pairing Type: Contrasting. Reasoning: The high fat content of the Cheddar effectively softens the high tannins of the Cabernet Sauvignon, while the wine's body matches the cheese's intensity.

---

**👤 You:**
> "Suggest some wines that pair well with a creamy, mild Brie."

**🤖 AI Agent:**
> Recommended wines: Chardonnay, Pinot Noir, and Sauvignon Blanc.

---

**👤 You:**
> "Is this profile valid: { 'profileType': 'wine', 'profileData': '{"grapeVariety": "Merlot", "region": "Bordeaux", "style": "dry", "body": "medium", "acidity": "medium", "tanninLevel": "medium", "sweetness": "dry", "alcoholPercent": 13.5}' }"

**🤖 AI Agent:**
> Yes, the profile is valid.


## ❓ FAQ

**Q: How is the pairing score calculated?**
The score is derived from deterministic rules including congruent matching, contrasting balance, regional bonuses, and chemical interactions like how acidity cuts through fat.

**Q: Can I validate my profile data before running a pairing?**
Yes, you can use the `validate_profiles` tool to ensure your wine or cheese profiles use the correct terminology and categories.

**Q: What if I want to find different wines for a specific cheese?**
You can use the `get_alternative_pairings` tool to suggest alternative wine profiles that meet a specific score threshold for your chosen cheese.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-cheese-pairing-engine](https://vinkius.com/ai-agent-connect/wine-cheese-pairing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine & Cheese Pairing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-cheese-pairing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine & Cheese Pairing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-cheese-pairing-engine": {
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
