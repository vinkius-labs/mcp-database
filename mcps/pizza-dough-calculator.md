# Pizza Dough Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pizza-dough-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Precise baker's percentage calculations for Neapolitan and NY style dough.

## Description
This MCP server provides professional-grade dough calculations using baker's percentages. It allows you to determine exact ingredient weights for flour, water, salt, and yeast based on your target hydration and dough ball size. Use `determine_yeast_dosage` to find the perfect yeast percentage for your specific fermentation time and temperature, and `calculate_recipe_ingredients` to get the final gram measurements. It also includes `generate_fermentation_schedule` to provide a complete timeline from mixing to final proofing, including adjustments for altitude.


## Available Tools (3)
- **calculate_recipe_ingredients**: Calculates the exact mass of every ingredient needed for a batch of dough
- **determine_yeast_dosage**: Determines the correct yeast percentage based on fermentation environment
- **generate_fermentation_schedule**: Provides a step-by-step timeline for the baker


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pizza Dough Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to make 10 dough balls of 250g each with 65% hydration. How much flour and water do I need?"

**🤖 AI Agent:**
> To make 10 dough balls of 250g at 65% hydration, you will need 1515.15g of flour and 984.85g of water.

---

**👤 You:**
> "What is the yeast percentage for a 24 hour room temperature fermentation at 20 degrees Celsius using instant yeast?"

**🤖 AI Agent:**
> For a 24-hour room temperature fermentation at 20°C using instant yeast, the required yeast percentage is 0.1%.

---

**👤 You:**
> "Give me a fermentation schedule for 300g dough balls using a cold retard method at 4 degrees Celsius."

**🤖 AI Agent:**
> For 300g dough balls with a cold retard at 4°C, your schedule is: mixing for 15 minutes, bulk fermentation for 2 hours, balling for 20 minutes, and a final proof of 24 hours.


## ❓ FAQ

**Q: How do I calculate the right amount of yeast?**
You can use the `determine_yeast_dosage` tool. Provide the fermentation method, duration, temperature, and yeast type to get the exact percentage needed.

**Q: Does this tool account for altitude?**
Yes, when using `calculate_recipe_ingredients`, you can provide the altitude in meters to automatically adjust the yeast weight.

**Q: Can I use this for Neapolitan dough?**
Yes, the tool is specifically designed for Neapolitan and New York style doughs using standard baker's percentages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pizza-dough-calculator](https://vinkius.com/ai-agent-connect/pizza-dough-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pizza Dough Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pizza-dough-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pizza Dough Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pizza-dough-calculator": {
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
