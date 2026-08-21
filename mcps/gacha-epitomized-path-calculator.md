# Gacha Epitomized Path Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gacha-epitomized-path-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate exact pull probabilities and resource costs for weapon banners.

## Description
This MCP server provides deterministic calculations for weapon banner mechanics. Use `calculate_probability` to find the chance of a target weapon appearing on the next 5-star pull, `calculate_expected_investment` to estimate the remaining pulls and primogem costs, and `validate_banner_state` to verify if your current pity and fate points are valid. It helps players plan their resource spending for specific target weapons.


## Available Tools (3)
- **calculate_expected_investment**: Calculates the estimated number of pulls and the total currency needed to guarantee the target weapon
- **calculate_probability**: Determines the likelihood of the user's target weapon appearing on their very next 5-star pull
- **validate_banner_state**: Confirms if the provided user data represents a valid and possible state within the system rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gacha Epitomized Path Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 50 pity pulls and 0 fate points. How many primogems do I need to guarantee my weapon?"

**🤖 AI Agent:**
> You will need 6400 primogems to guarantee your target weapon.

---

**👤 You:**
> "What is my probability of getting the weapon if I have 1 fate point?"

**🤖 AI Agent:**
> Your probability of getting the target weapon on the next 5-star pull is 0.75.

---

**👤 You:**
> "Is it possible to have 95 pity pulls?"

**🤖 AI Agent:**
> No, the maximum hard pity threshold is 90 pulls.


## ❓ FAQ

**Q: How do I know if my state is valid?**
You can use the `validate_banner_state` tool to check if your current pity pulls (0-90) and fate points (0-2) are logically possible.

**Q: How much will it cost to get my target weapon?**
Use the `calculate_expected_investment` tool. It calculates the expected remaining pulls and multiplies them by 160 to give you the total primogem cost.

**Q: What is my chance of success on the next 5-star?**
The `calculate_probability` tool will tell you your exact chance. If you have 2 fate points, your chance is 1.0 (100%).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gacha-epitomized-path-calculator](https://vinkius.com/ai-agent-connect/gacha-epitomized-path-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gacha Epitomized Path Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gacha-epitomized-path-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gacha Epitomized Path Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gacha-epitomized-path-calculator": {
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
