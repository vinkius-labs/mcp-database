# Tire Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tire-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate tire dimensions, speedometer error, and clearance risks.

## Description
An essential tool for automotive enthusiasts and professionals to precisely calculate tire geometry. Use `calculate_tire_dimensions` to get physical profiles from metric notation, `calculate_speedometer_deviation` to understand how new tires impact your dashboard reading, and `evaluate_clearance_compatibility` to identify potential mechanical rubbing risks when upgrading sizes.


## Available Tools (3)
- **calculate_speedometer_deviation**: Calculates speedometer error when changing tire sizes
- **calculate_tire_dimensions**: Returns width, sidewall height, diameter, circumference, and revs per mile.

Calculates physical dimensions of a tire
- **evaluate_clearance_compatibility**: Checks for potential tire rubbing/interference


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tire Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dimensions for a 265/70R17 tire?"

**🤖 AI Agent:**
> For a 265/70R17 tire, the width is 265mm (10.43in), sidewall height is 185.5mm (7.30in), and overall diameter is 773.1mm (30.44in).

---

**👤 You:**
> "If I switch from 265/70R17 to 285/75R18, what is the speedometer error?"

**🤖 AI Agent:**
> The speedometer error will be approximately -3.45%, meaning your actual speed will be slightly higher than what is shown.

---

**👤 You:**
> "Is a 780mm diameter tire safe to install if my current is 720mm and threshold is 25mm?"

**🤖 AI Agent:**
> The diameter delta is 60mm. This exceeds your 25mm threshold, indicating a High Risk of mechanical interference.


## ❓ FAQ

**Q: How do I calculate the diameter of my new tire?**
You can use the `calculate_tire_dimensions` tool by providing the metric size, such as '265/70R17'.

**Q: Will my speedometer be accurate after changing tires?**
Changing tire sizes can cause deviation. Use `calculate_speedometer_deviation` to find the exact error percentage.

**Q: How can I check if larger tires will rub against my car?**
Use the `evaluate_clearance_compatibility` tool with your current and new diameters to assess mechanical risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tire-size-converter](https://vinkius.com/mcp/tire-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tire Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tire-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tire Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tire-size-converter": {
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
