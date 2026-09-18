# Lean Body Mass Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lean-body-mass-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate lean body mass, fat mass, and protein requirements.

## Description
This MCP server provides precise body composition analysis. Use `get_composition_summary` to receive a complete profile including lean body mass, fat mass, muscularity index, and daily protein needs. It also offers individual tools like `calculate_body_composition` for mass breakdown, `calculate_muscularity_index` for height-relative mass assessment, and `calculate_protein_needs` for dietary planning.


## Available Tools (4)
- **calculate_body_composition**: Provides a fundamental breakdown of body mass into fat and lean components
- **calculate_muscularity_index**: Evaluates how much lean mass an individual carries relative to their height
- **calculate_protein_needs**: Determines the daily protein intake required to maintain current lean muscle mass
- **get_composition_summary**: Provides a complete overview of all calculated body metrics in a single call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lean Body Mass Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a full body composition summary for a person weighing 85kg, with 15% body fat, 1.8 meters tall, and they are an athlete."

**🤖 AI Agent:**
> Based on your metrics, your lean body mass is 72.25 kg, your fat mass is 12.75 kg, your muscularity index is 40.14, and your daily protein requirement is 144.5 grams.

---

**👤 You:**
> "Calculate the protein needs for someone with 60kg of lean body mass."

**🤖 AI Agent:**
> The daily protein requirement for 60kg of lean body mass is 60.0 grams.

---

**👤 You:**
> "What is the fat mass for a 70kg person with 25% body fat?"

**🤖 AI Agent:**
> The fat mass is 17.5 kg.


## ❓ FAQ

**Q: How do I get a full body profile?**
You can use the `get_composition_summary` tool to get all metrics like lean mass, fat mass, and protein needs in one response.

**Q: Does this account for athletes?**
Yes, the `calculate_protein_needs` tool includes an option to adjust protein requirements for athletic populations.

**Q: What units are used for measurements?**
Weight is measured in kilograms and height is measured in meters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lean-body-mass-calculator](https://vinkius.com/en/ai-agent-connect/lean-body-mass-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lean Body Mass Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lean-body-mass-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lean Body Mass Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lean-body-mass-calculator": {
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
