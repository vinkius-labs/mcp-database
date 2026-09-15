# Surf Session Calorie Burn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-session-calorie-burn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate calories burned during surfing sessions based on intensity and activity breakdown.

## Description
This MCP server provides specialized tools to estimate energy expenditure for surfers. By accounting for the metabolic difference between paddling and riding waves, it calculates total calories burned, hourly burn rates, and specific energy expenditure for each activity type. Use `calculate_session_metrics` for a full session overview, `get_intensity_reference` to understand MET values, `compare_session_intensities` to see how intensity changes impact burn, and `estimate_weight_impact` to see how body mass affects your results.


## Available Tools (4)
- **calculate_session_metrics**: Provides a comprehensive overview of the caloric cost of a specific surf session
- **compare_session_intensities**: Answers "How much more energy will I burn if I surf more intensely?"
- **estimate_weight_impact**: Answers "How does my body weight affect my calorie burn at a specific intensity?"
- **get_intensity_reference**: Allows the user to understand which intensity level to choose for their calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Session Calorie Burn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories will I burn in a 60 minute surf session if I weigh 80kg and spend 70% of the time paddling at moderate intensity?"

**🤖 AI Agent:**
> For a 60-minute session at moderate intensity with an 80kg weight and 70% paddling ratio, you will burn approximately 450 calories.

---

**👤 You:**
> "What are the different intensity levels available?"

**🤖 AI Agent:**
> The available intensity levels are Low, Moderate, High, and Extreme, each with different metabolic equivalent values.

---

**👤 You:**
> "How much more energy would I burn if I switched from moderate to high intensity for a 45 minute session at 75kg?"

**🤖 AI Agent:**
> Switching from moderate to high intensity for a 45-minute session at 75kg would increase your calorie burn by approximately 120 calories.


## ❓ FAQ

**Q: How do I know which intensity level to select?**
You can use the `get_intensity_reference` tool to view a detailed list of intensity levels, their descriptions, and their corresponding metabolic equivalent (MET) values.

**Q: Does the calculation account for the time spent paddling?**
Yes, the `calculate_session_metrics` tool uses a paddling ratio to distinguish between steady-state paddling and high-intensity wave riding.

**Q: How much does my weight affect the results?**
Body weight is a key factor in energy expenditure. You can use `estimate_weight_impact` to see exactly how much your weight influences the total calories burned.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-session-calorie-burn](https://vinkius.com/en/ai-agent-connect/surf-session-calorie-burn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Session Calorie Burn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-session-calorie-burn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Session Calorie Burn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-session-calorie-burn": {
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
