# Fragrance Spray Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fragrance-spray-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate total sprays, usage duration, and bottle efficiency for fragrance products.

## Description
This MCP server provides precise calculations for fragrance bottle capacity and usage. Use `get_spray_capacity` to find the total number of sprays available in a bottle, or `calculate_usage_projection` to estimate how many days a fragrance will last based on your daily spray habits. You can also use `validate_dosage_safety` to check if a spray volume is within standard industry ranges and `get_bottle_efficiency_rating` to assess the longevity of a bottle.


## Available Tools (4)
- **calculate_usage_projection**: Estimates how many days a bottle will last based on daily usage habits
- **get_bottle_efficiency_rating**: Compares the bottle volume against the spray volume to provide a qualitative assessment of longevity
- **get_spray_capacity**: Calculates the total number of sprays possible from a given bottle volume
- **validate_dosage_safety**: Checks if a specific spray volume is within realistic/safe manufacturing ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fragrance Spray Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many sprays are in a 50ml bottle if each spray is 0.1ml?"

**🤖 AI Agent:**
> There are 500 sprays available in a 50ml bottle with a 0.1ml spray volume.

---

**👤 You:**
> "If I have a 100ml bottle and spray 3 times a day with a 0.12ml spray, how many days will it last?"

**🤖 AI Agent:**
> The fragrance will last for approximately 277 days.

---

**👤 You:**
> "Is a 0.5ml spray volume standard for fragrance?"

**🤖 AI Agent:**
> No, a 0.5ml spray volume is considered unusually high for standard fragrance atomizers.


## ❓ FAQ

**Q: How do I calculate how long my perfume will last?**
You can use the `calculate_usage_projection` tool by providing the bottle volume, the volume per spray, and how many times you spray per day.

**Q: Can I check if a spray volume is standard?**
Yes, the `validate_dosage_safety` tool checks if a specific spray volume is within realistic manufacturing ranges for standard atomizers.

**Q: What is the total number of sprays in a 100ml bottle?**
To find this, use `get_spray_capacity` with a bottle volume of 100ml and your specific spray volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fragrance-spray-calculator](https://vinkius.com/en/ai-agent-connect/fragrance-spray-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fragrance Spray Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fragrance-spray-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fragrance Spray Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fragrance-spray-calculator": {
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
