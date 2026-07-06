# Baby Bottle Feeding Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baby-bottle-feeding-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generate precise 24-hour infant feeding schedules and monthly formula inventory predictions.

## Description
This MCP server provides essential tools for parents and caregivers to manage infant nutrition. Using `calculate_daily_volume_target`, you can determine the total daily formula requirement based on an infant's weight in kilograms or pounds. The `generate_feeding_schedule` tool creates a detailed 24-hour feeding plan, allowing for custom intervals and a 'bedtime boost' to adjust the final feed volume. Additionally, `calculate_monthly_supply` helps with long-term planning by predicting how many cans of formula powder are needed per month based on your baby's specific nutritional needs and scoop-to-ml ratios.


## Available Tools (3)
- **generate_feeding_schedule**: Generate a 24-hour feeding schedule
- **calculate_monthly_supply**: Calculate formula cans needed per month
- **calculate_daily_volume_target**: Calculate the total daily feeding volume based on infant weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baby Bottle Feeding Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My baby weighs 5kg. How much formula do they need daily?"

**🤖 AI Agent:**
> Based on a weight of 5kg, your baby requires a total daily volume of 750ml.

---

**👤 You:**
> "Create a feeding schedule for 750ml daily, every 3 hours, starting at 6:00 AM."

**🤖 AI Agent:**
> Your 24-hour schedule is: 06:00 - 125ml, 09:00 - 125ml, 12:00 - 125ml, 15:00 - 125ml, 18:00 - 125ml, 21:00 - 125ml, 00:00 - 125ml.

---

**👤 You:**
> "How many cans of formula do I need for a month if my baby needs 750ml daily, one scoop makes 30ml, and a can has 90 scoops?"

**🤖 AI Agent:**
> You will need 3 cans of formula per month.


## ❓ FAQ

**Q: How is the daily volume calculated?**
The `calculate_daily_volume_target` tool uses a standard requirement of 150ml of formula per kilogram of infant weight daily.

**Q: Can I adjust the last feed of the day?**
Yes, using `generate_feeding_schedule`, you can apply a 'bedtime boost factor' to increase the volume of the final feeding.

**Q: How do I estimate formula usage for the month?**
Use the `calculate_monthly_supply` tool by providing your daily target volume, the ml produced per scoop, and the total scoops per can.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baby-bottle-feeding-scheduler](https://vinkius.com/mcp/baby-bottle-feeding-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baby Bottle Feeding Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baby-bottle-feeding-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baby Bottle Feeding Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baby-bottle-feeding-scheduler": {
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
