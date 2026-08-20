# Matcha Ceremony Parameter Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/matcha-ceremony-parameter-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate precise matcha recipes, water temperatures, and caffeine estimates.

## Description
This MCP server provides deterministic calculations for traditional Japanese matcha preparation. It helps users determine the exact powder weight, water volume, and whisking time required for different styles like Usucha or Koicha. Use `calculate_preparation_parameters` to get a complete recipe, `validate_temperature_profile` to ensure your water temperature matches your matcha grade, and `estimate_caffeine_intake` to track caffeine consumption.


## Available Tools (3)
- **calculate_preparation_parameters**: Determines the precise recipe (powder, water, time) for a specific matcha session
- **estimate_caffeine_intake**: Provides a caffeine estimation based on the weight of matcha being consumed
- **validate_temperature_profile**: Checks if the user's water temperature is optimal for their chosen matcha grade


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matcha Ceremony Parameter Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make Usucha with ceremonial grade matcha using 75°C water. What is the recipe?"

**🤖 AI Agent:**
> For your ceremonial Usucha, use 1.8g of matcha powder and 65ml of water. Whisk for 20 seconds.

---

**👤 You:**
> "Is 82°C water okay for premium grade matcha?"

**🤖 AI Agent:**
> Yes, 82°C is within the optimal range for premium grade matcha.

---

**👤 You:**
> "How much caffeine is in 4 grams of matcha?"

**🤖 AI Agent:**
> 4 grams of matcha contains approximately 140mg of caffeine.


## ❓ FAQ

**Q: How do I know if my water temperature is correct?**
You can use the `validate_temperature_profile` tool. It checks your water temperature against the optimal range for ceremonial, premium, or culinary grades.

**Q: What is the difference between Usucha and Koicha?**
Usucha is a thin, frothy tea with more water, while Koicha is a thick, dense tea with more powder. The `calculate_preparation_parameters` tool provides specific ratios for both.

**Q: Can I estimate caffeine content?**
Yes, use the `estimate_caffeine_intake` tool by providing the weight of the matcha powder used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/matcha-ceremony-parameter-calculator](https://vinkius.com/ai-agent-connect/matcha-ceremony-parameter-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Matcha Ceremony Parameter Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `matcha-ceremony-parameter-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Matcha Ceremony Parameter Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "matcha-ceremony-parameter-calculator": {
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
