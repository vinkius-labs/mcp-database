# Capsule Wardrobe Gap Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-gap-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify missing clothing items needed to meet outfit goals, color rules, and climate needs.

## Description
This MCP server acts as a specialized gap-analysis engine for sustainable fashion. It evaluates your current clothing inventory against specific outfit goals, color palettes, and weather constraints. By using `identify_wardrobe_gaps`, you can find exactly which items are missing to satisfy your desired outfit combinations and minimum-use targets. It also includes tools like `validate_color_rules` to ensure aesthetic consistency and `evaluate_climate_suitability` to verify thermal appropriateness for your target weather.


## Available Tools (4)
- **calculate_wear_efficiency**: Measures how well the current wardrobe meets the sustainability goal of frequent use
- **evaluate_climate_suitability**: Determines if a specific outfit is appropriate for the intended weather
- **identify_wardrobe_gaps**: Find specific items missing to complete the user's intended capsule
- **validate_color_rules**: Checks if a proposed set of items adheres to the user's specific aesthetic constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capsule Wardrobe Gap Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a few blue tops and black bottoms. What am I missing to create 5 professional outfits for a cold climate?"

**🤖 AI Agent:**
> To meet your goal of 5 professional outfits in a cold climate, you are missing: 1x Heavyweight Grey Coat, 1x Navy Wool Sweater, and 1x Black Thermal Base Layer.

---

**👤 You:**
> "Is this outfit suitable for a tropical climate: a linen shirt and cotton shorts?"

**🤖 AI Agent:**
> Yes, the combination of a linen shirt and cotton shorts is suitable for a tropical climate.

---

**👤 You:**
> "Check if my navy blazer and black trousers follow my rule that navy cannot be paired with black."

**🤖 AI Agent:**
> The combination violates your rule: Navy cannot be paired with Black.


## ❓ FAQ

**Q: How do I find out what clothes I am missing?**
You can use the `identify_wardrobe_gaps` tool by providing your current inventory, desired outfit goals, and color palette.

**Q: Can I check if my outfits are warm enough for winter?**
Yes, the `evaluate_climate_suitability` tool checks if your outfit items meet the thermal requirements for your target climate.

**Q: How does the tool handle color constraints?**
The `validate_color_rules` tool allows you to define specific aesthetic constraints to ensure your items pair correctly according to your rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-gap-analyzer](https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-gap-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Capsule Wardrobe Gap Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `capsule-wardrobe-gap-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Capsule Wardrobe Gap Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capsule-wardrobe-gap-analyzer": {
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
