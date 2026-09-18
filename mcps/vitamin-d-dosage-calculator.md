# Vitamin D Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vitamin-d-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized Vitamin D supplementation strategies based on physiological and environmental factors.

## Description
This MCP server provides precise Vitamin D supplementation roadmaps. By analyzing physiological data like BMI and skin type alongside environmental factors like latitude and season, it calculates specific needs. Use `get_personalized_dosage_plan` for a complete roadmap, `get_daily_requirement` for maintenance doses, or `calculate_loading_strategy` to address severe deficiencies.


## Available Tools (4)
- **calculate_loading_strategy**: Determines if a loading dose is necessary and defines the dosage and duration to reach target levels
- **get_daily_requirement**: Calculates the standard daily maintenance dose required to sustain optimal Vitamin D levels
- **get_environmental_uv_factor**: Calculates the efficiency of natural Vitamin D synthesis based on location and time
- **get_personalized_dosage_plan**: Provides a complete, unified supplementation roadmap including loading and maintenance phases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vitamin D Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you create a Vitamin D plan for me? My current level is 15 ng/mL, target is 40 ng/mL, BMI is 26, skin type is 3, I get 4 hours of sun per week, live at latitude 40, and it is currently winter."

**🤖 AI Agent:**
> Your personalized plan includes a loading phase of 50,000 IU daily for 8 days, followed by a maintenance dose of 2,000 IU daily to maintain your target level.

---

**👤 You:**
> "What is my daily maintenance dose for Vitamin D? I have a BMI of 22, skin type 2, 10 hours of sun exposure, latitude 35, and it is summer. My current level is 30 ng/mL."

**🤖 AI Agent:**
> Your recommended daily maintenance dose is 1,500 IU.

---

**👤 You:**
> "I need to know if I need a loading dose. My current level is 10 ng/mL, target is 35 ng/mL, and my BMI is 30."

**🤖 AI Agent:**
> Yes, a loading dose is required. You should take 50,000 IU daily for 10 days to reach your target level.


## ❓ FAQ

**Q: How does skin type affect the calculation?**
The tool uses the Fitzpatrick skin scale to adjust for melanin levels, which influence how efficiently your skin synthesizes Vitamin D from sunlight.

**Q: What is a loading dose?**
A loading dose is a higher initial amount of Vitamin D used to rapidly correct a deficiency before transitioning to a maintenance dose.

**Q: Does BMI impact the recommended dose?**
Yes, because Vitamin D is fat-soluble, higher BMI values may require higher doses to reach optimal serum levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vitamin-d-dosage-calculator](https://vinkius.com/en/ai-agent-connect/vitamin-d-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vitamin D Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vitamin-d-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vitamin D Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vitamin-d-dosage-calculator": {
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
