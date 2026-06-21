# Temperature Converter for Cooking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/temperature-converter-for-cooking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert oven temperatures between Celsius, Fahrenheit, and the European Gas scale with heat intensity classification.

## Description
This MCP server provides precise temperature conversions for cooking environments. It allows AI agents to convert between Celsius, Fahrenheit, and the European Gas oven scale (1-9). Beyond simple unit conversion, it also classifies the heat intensity as Low, Medium, High, or Very High based on the resulting temperature. Use tools like `fahrenheit_from_celsius`, `celsius_from_fahrenheit`, and `oven_settings_from_gas` to get accurate cooking instructions.


## Available Tools (3)
- **celsius_from_fahrenheit**: Convert Fahrenheit to Celsius
- **fahrenheit_from_celsius**: Convert Celsius to Fahrenheit
- **oven_settings_from_gas**: Get oven settings from gas knob position


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temperature Converter for Cooking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is 180 degrees Celsius in Fahrenheit?"

**🤖 AI Agent:**
> 180°C is approximately 356°F, which corresponds to a High heat level.

---

**👤 You:**
> "Convert gas setting 4 to Celsius."

**🤖 AI Agent:**
> Gas setting 4 corresponds to approximately 150°C (302°F), which is a Medium heat level.

---

**👤 You:**
> "What temperature is 400 Fahrenheit in Celsius?"

**🤖 AI Agent:**
> 400°F is approximately 204.4°C, which falls under the Very High heat level.


## ❓ FAQ

**Q: How can I convert Celsius to Fahrenheit?**
You can use the `fahrenheit_from_celsius` tool by providing the temperature in degrees Celsius.

**Q: What is the European Gas scale?**
The Gas scale is a numbering system (1-9) used in many European gas ovens. The `oven_settings_from_gas` tool maps these settings to Celsius and Fahrenheit.

**Q: Does it provide heat intensity information?**
Yes. Every conversion result includes a heat level classification: Low, Medium, High, or Very High.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temperature-converter-for-cooking](https://vinkius.com/mcp/temperature-converter-for-cooking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Temperature Converter for Cooking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `temperature-converter-for-cooking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Temperature Converter for Cooking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "temperature-converter-for-cooking": {
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
