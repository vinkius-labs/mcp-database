# Barbecue Meat Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/barbecue-meat-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic planning for BBQ meat procurement, cooking times, and fuel needs.

## Description
Plan your next barbecue with precision. This MCP server provides a deterministic engine to calculate exactly how much raw meat to buy, how long each cut needs to cook, and how much fuel you will consume. Use `calculate_meat_requirements` to determine procurement needs based on guest count and appetite, `calculate_cooking_schedule` to map out your cook time and fuel, and `get_thermal_targets` to ensure every piece of meat reaches its ideal internal temperature.


## Available Tools (3)
- **calculate_cooking_schedule**: Calculate cooking schedule and fuel requirements
- **calculate_meat_requirements**: Calculate raw meat requirements based on guests, appetite, and style
- **get_thermal_targets**: Get target internal temperatures for specific meat types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Barbecue Meat Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much brisket and pork shoulder should I buy for 10 average eaters for a main dish?"

**🤖 AI Agent:**
> For 10 average eaters serving a main dish, you should purchase 12.5kg of brisket and 9.4kg of pork shoulder.

---

**👤 You:**
> "What is the cooking schedule for 5lbs of brisket?"

**🤖 AI Agent:**
> For 5lbs of brisket, the estimated cook time is 6.25 hours, requiring 12.5kg of fuel, with a recommended resting time of 45 minutes.

---

**👤 You:**
> "What internal temperature should I aim for with chicken?"

**🤖 AI Agent:**
> The target internal temperature for chicken is 165°F (74°C).


## ❓ FAQ

**Q: How does the calculator handle meat shrinkage?**
The engine uses specific yield factors for different meats. For example, brisket has a 50% yield, meaning you must buy twice the weight you intend to serve.

**Q: Can I plan for bone-in meats?**
Yes. When using `calculate_meat_requirements`, you can specify if the meat is bone-in to ensure the raw weight accounts for the non-edible bone mass.

**Q: How is fuel consumption calculated?**
The `calculate_cooking_schedule` tool estimates fuel needs by calculating 2kg of wood or charcoal per hour of total cooking time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/barbecue-meat-calculator](https://vinkius.com/ai-agent-connect/barbecue-meat-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Barbecue Meat Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `barbecue-meat-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Barbecue Meat Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "barbecue-meat-calculator": {
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
