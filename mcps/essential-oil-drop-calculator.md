# Essential Oil Drop Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/essential-oil-drop-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate the exact number of essential oil drops needed for a specific dilution percentage in any carrier oil volume.

## Description
The Essential Oil Drop Calculator provides precise instructions for safe essential oil dilution. By using tools like `calculate_drops_needed`, you can determine exactly how many drops to add to your carrier oil volume (in ml) to reach a target concentration. It also allows you to verify existing mixtures with `check_dilution_safety` and understand the total capacity of your bottle via `get_drop_capacity_info`. This ensures consistent, safe, and accurate dilution for all your aromatherapy needs.


## Available Tools (3)
- **calculate_drops_needed**: g., 1% or 2%). It returns exactly how many drops to add.

Calculates how many drops of essential oil to add to a carrier oil volume
- **check_dilution_safety**: Checks if a current mixture of essential oil and carrier oil is at a safe dilution level
- **get_drop_capacity_info**: Retrieves the total drop capacity for a specific volume of carrier oil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Essential Oil Drop Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many drops of essential oil should I add to 30ml of jojoba oil for a 2% dilution?"

**🤖 AI Agent:**
> You should add 1 drop of essential oil to your 30ml of jojoba oil to achieve a 2% dilution.

---

**👤 You:**
> "Is my mixture safe? I added 5 drops to 10ml of almond oil."

**🤖 AI Agent:**
> Your current dilution is 2.5%. This falls into the Strong category, which may require caution for certain skin types.

---

**👤 You:**
> "How many total drops are in a 50ml bottle of coconut oil?"

**🤖 AI Agent:**
> A 50ml volume of coconut oil contains exactly 1,000 drops.


## ❓ FAQ

**Q: How does the calculator determine the number of drops?**
The tool uses a standard conversion where 1 ml is equal to 20 drops. It calculates the total drop capacity of your carrier oil and then determines the specific number of drops required to reach your target percentage.

**Q: Can I check if my current mixture is safe?**
Yes, you can use the `check_dilution_safety` tool. Simply provide the volume of carrier oil and the number of drops already added to see if your mixture falls within standard safety ranges.

**Q: What is a standard dilution percentage?**
For most skin applications, a concentration between 1% and 2% is considered standard. The calculator helps you stay within these safe boundaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/essential-oil-drop-calculator](https://vinkius.com/mcp/essential-oil-drop-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Essential Oil Drop Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `essential-oil-drop-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Essential Oil Drop Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "essential-oil-drop-calculator": {
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
