# Fragrance Cost per Spray MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fragrance-cost-per-spray)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the precise cost of every individual fragrance spray.

## Description
This MCP server provides specialized tools to analyze the unit economics of perfumes and colognes. By determining the cost per single actuation of the atomizer, users can accurately compare the value of different fragrances regardless of bottle size or price. Use `calculate_spray_economics` to find the cost per spray, `estimate_spray_capacity` to predict total sprays from a volume, `compare_fragrance_value` to identify the most economical option, and `calculate_usage_lifespan` to estimate how many days a bottle will last based on daily habits.


## Available Tools (4)
- **calculate_spray_economics**: Calculate the cost per spray and liquid value
- **calculate_usage_lifespan**: Calculate how many days a bottle will last
- **compare_fragrance_value**: Compare the cost per spray of two different fragrances
- **estimate_spray_capacity**: Estimate the total number of sprays available in a bottle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fragrance Cost per Spray** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought a 100ml bottle for $120 that has 1200 sprays. What is the cost per spray?"

**🤖 AI Agent:**
> The cost per spray is $0.10.

---

**👤 You:**
> "How many sprays are in a 50ml bottle if each spray is 0.1ml?"

**🤖 AI Agent:**
> There are 500 sprays in a 50ml bottle.

---

**👤 You:**
> "If I have 1000 sprays and I use 4 sprays every day, how many days will it last?"

**🤖 AI Agent:**
> The bottle will last for 250 days.


## ❓ FAQ

**Q: How is the cost per spray calculated?**
The cost per spray is calculated by dividing the total purchase price of the fragrance by the estimated number of sprays available in the bottle using `calculate_spray_economics`.

**Q: Can I compare two different perfumes?**
Yes, you can use the `compare_fragrance_value` tool to determine which fragrance is more economical based on the cost per spray.

**Q: How can I know how long my bottle will last?**
You can use `calculate_usage_lifespan` by providing the total number of sprays and your average daily usage rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fragrance-cost-per-spray](https://vinkius.com/en/ai-agent-connect/fragrance-cost-per-spray)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fragrance Cost per Spray** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fragrance-cost-per-spray` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fragrance Cost per Spray** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fragrance-cost-per-spray": {
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
