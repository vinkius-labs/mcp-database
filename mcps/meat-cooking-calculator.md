# Meat Cooking Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/meat-cooking-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Precise cooking times, temperatures, and resting requirements for various meats.

## Description
This MCP server provides deterministic culinary calculations to ensure perfect results every time. Use `calculate_cooking_parameters` to generate a complete plan including target internal temperatures, estimated cooking duration, and necessary resting time. You can also use `get_temperature_guidelines` to find specific temperature ranges for different doneness levels, or `validate_cooking_safety` to verify that your target temperature meets food safety standards. It accounts for weight, cooking method, bone-in status, and even altitude adjustments.


## Available Tools (3)
- **calculate_cooking_parameters**: Calculates specific temperature targets, cooking duration, and resting requirements
- **get_temperature_guidelines**: Retrieves standard internal temperature ranges for a meat type and doneness
- **validate_cooking_safety**: Checks if a planned cooking temperature meets food safety requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meat Cooking Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 2kg beef roast that is bone-in. I want to cook it in the oven to medium-rare. How long will it take and what temperature should I aim for?"

**🤖 AI Agent:**
> For a 2kg bone-in beef roast cooked in the oven to medium-rare, you should aim for an internal temperature of 130-135°F. The estimated cooking time is 145 minutes, and you should let it rest for 15 minutes.

---

**👤 You:**
> "What is the safe temperature for chicken?"

**🤖 AI Agent:**
> The minimum safe internal temperature for chicken is 165°F.

---

**👤 You:**
> "Is 140°F safe for a pork chop?"

**🤖 AI Agent:**
> No, 140°F is below the required safety threshold for pork. You should ensure it reaches the recommended minimum temperature to ensure it is safe to eat.


## ❓ FAQ

**Q: How does altitude affect my cooking time?**
The calculator automatically adjusts the estimated cooking time by increasing it 5% for every 1000 meters of altitude to account for changes in heat transfer efficiency.

**Q: Can I use this for poultry?**
Yes. While doneness levels are primarily for red meats, the tools provide the necessary safety minimum temperatures for chicken and turkey.

**Q: What is carryover cooking?**
Carryover cooking is the rise in internal temperature that occurs after meat is removed from the heat source. The `calculate_cooking_parameters` tool provides an estimate of this rise.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/meat-cooking-calculator](https://vinkius.com/ai-agent-connect/meat-cooking-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meat Cooking Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meat-cooking-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meat Cooking Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meat-cooking-calculator": {
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
