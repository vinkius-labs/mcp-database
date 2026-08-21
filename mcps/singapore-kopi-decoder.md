# Singapore Kopi Decoder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-kopi-decoder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Translates Singaporean coffee shorthand and calculates nutritional data.

## Description
This MCP server acts as a bridge between users and the complex dialect-based shorthand of Singaporean coffee (Kopi) and tea (Teh) culture. It provides tools to translate colloquial orders like 'Kopi C Siew Dai Peng' into standardized English, validate if the order is logically consistent, and estimate calories and sugar reduction based on local health standards. Use `translate_order` to get a formal description, `calculate_nutrition` for calorie estimates, and `validate_order_consistency` to check for conflicting modifiers.


## Available Tools (3)
- **calculate_nutrition**: Estimates the nutritional impact of the specific drink order
- **translate_order**: Translates colloquial Kopi/Teh shorthand into a standardized English description and validates the logic of the request
- **validate_order_consistency**: A specialized check to ensure the user hasn't provided a contradictory or physically impossible order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore Kopi Decoder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Kopi Kosong Peng' for me."

**🤖 AI Agent:**
> Coffee, no sugar, iced.

---

**👤 You:**
> "How many calories are in a 'Teh C Siew Dai'?"

**🤖 AI Agent:**
> The estimated calorie count for Teh C Siew Dai is 120 calories.

---

**👤 You:**
> "Is 'Milo Siew Dai Kosong' a valid order?"

**🤖 AI Agent:**
> No, that order is invalid because 'Siew Dai' (less sugar) and 'Kosong' (no sugar) are conflicting sugar levels.


## ❓ FAQ

**Q: What does 'C' mean in a Kopi order?**
'C' indicates that the drink uses evaporated milk instead of the traditional condensed milk.

**Q: How are calories calculated?**
Calories are estimated using the `calculate_nutrition` tool, which applies fixed local health standards to the base liquid and selected modifiers.

**Q: Can I check if my order is valid?**
Yes, you can use the `validate_order_consistency` tool to ensure you haven't requested conflicting modifiers, such as 'Kosong' and 'Siew Dai' together.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-kopi-decoder](https://vinkius.com/ai-agent-connect/singapore-kopi-decoder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore Kopi Decoder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-kopi-decoder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore Kopi Decoder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-kopi-decoder": {
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
