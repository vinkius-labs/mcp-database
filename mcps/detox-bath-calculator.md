# Detox Bath Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/detox-bath-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate optimal Epsom salt concentrations and bath recipes tailored to your physical profile.

## Description
This MCP server provides precise calculations for Epsom salt baths. Use `recommend_bath_composition` to get a complete recipe including salt mass, additives, temperature, and soak duration based on your body weight and skin sensitivity. You can also use `calculate_salt_requirement` to find the exact amount of salt needed for a specific tub volume, or `validate_safety_limits` to ensure your bath configuration is safe for your skin type.


## Available Tools (4)
- **calculate_salt_requirement**: Determines the exact mass of Epsom salt needed to achieve a target concentration in a specific tub volume
- **get_absorption_estimate**: Estimates the physiological impact/absorption potential of the bath
- **recommend_bath_composition**: Provides a complete recipe including salt, additives, temperature, and duration based on the user's physical profile
- **validate_safety_limits**: Checks if a proposed bath configuration is safe for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Detox Bath Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 150 liter tub and want a standard concentration. What is the salt requirement?"

**🤖 AI Agent:**
> For a 150 liter tub at your target concentration, you will need 4500 grams of Epsom salt.

---

**👤 You:**
> "Recommend a bath for a 70kg person with medium skin sensitivity for a 100 liter tub."

**🤖 AI Agent:**
> For your profile, use 1500g of Epsom salt, 20g of baking soda, and 5 drops of essential oils. Soak at 37°C for 20 minutes.

---

**👤 You:**
> "Is a 45°C bath with high salt concentration safe for someone with high skin sensitivity?"

**🤖 AI Agent:**
> No, that configuration is unsafe. High skin sensitivity requires lower temperatures and lower concentrations to prevent irritation.


## ❓ FAQ

**Q: How do I know if my bath is safe?**
You can use the `validate_safety_limits` tool to check if your intended salt concentration and water temperature are safe for your specific skin sensitivity level.

**Q: Can I get a full recipe for my bath?**
Yes, the `recommend_bath_composition` tool provides a full recipe including salt mass, baking soda, essential oil drops, temperature, and duration.

**Q: How much salt do I need for my tub?**
Use the `calculate_salt_requirement` tool by providing your tub volume and desired concentration to find the exact mass required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/detox-bath-calculator](https://vinkius.com/en/ai-agent-connect/detox-bath-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Detox Bath Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `detox-bath-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Detox Bath Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "detox-bath-calculator": {
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
