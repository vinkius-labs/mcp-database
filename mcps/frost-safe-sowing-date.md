# Frost-Safe Sowing Date MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/frost-safe-sowing-date)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise indoor and outdoor sowing dates based on frost patterns.

## Description
This MCP server provides precision timing for gardeners and farmers. It calculates the ideal windows for starting seeds indoors or planting directly outdoors by analyzing the last frost date against specific crop requirements. Use `get_crop_growth_requirements` to find standard growth parameters, `calculate_outdoor_sowing_date` for direct planting, or `calculate_indoor_sowing_date` to prepare seedlings for transplanting. You can also use `compare_planting_windows` to decide which method fits your seasonal timeline best.


## Available Tools (4)
- **calculate_indoor_sowing_date**: Determines when a user should start seeds indoors to prepare them for outdoor transplanting
- **get_crop_growth_requirements**: Retrieves the standard growth parameters for a specific type of crop
- **calculate_outdoor_sowing_date**: Determines when a user can plant seeds directly into the soil to ensure they mature before the frost
- **compare_planting_windows**: Compares the outdoor and indoor options to help a user decide which method is more feasible for their timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frost-Safe Sowing Date** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the growth requirements for a tomato?"

**🤖 AI Agent:**
> For a tomato, the standard requirements are 8 weeks before frost, 7 days for germination, and 10 days for hardening.

---

**👤 You:**
> "When should I plant seeds outdoors if the last frost is 2024-05-15 and my crop needs 6 weeks of growth?"

**🤖 AI Agent:**
> You should plant your seeds outdoors on 2024-04-03.

---

**👤 You:**
> "Calculate my indoor sowing date for a crop needing 5 weeks of growth, 5 days to germinate, and 7 days to harden, with a last frost of 2024-05-15."

**🤖 AI Agent:**
> Your indoor sowing date is 2024-03-25.


## ❓ FAQ

**Q: How do I find the growth requirements for my specific plant?**
You can use the `get_crop_growth_requirements` tool to retrieve standard weeks before frost, germination days, and hardening days for common crops like tomatoes or lettuce.

**Q: What is the difference between indoor and outdoor sowing?**
Outdoor sowing is direct planting in the ground, while indoor sowing involves starting seeds in a controlled environment to allow for germination and hardening before the frost-free period begins.

**Q: Can I compare both planting methods?**
Yes, the `compare_planting_windows` tool provides both dates and the difference in days to help you choose the best method.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/frost-safe-sowing-date](https://vinkius.com/en/ai-agent-connect/frost-safe-sowing-date)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frost-Safe Sowing Date** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `frost-safe-sowing-date` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frost-Safe Sowing Date** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frost-safe-sowing-date": {
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
