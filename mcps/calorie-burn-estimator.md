# Calorie Burn Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calorie-burn-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate energy expenditure using MET values, body weight, and activity duration.

## Description
The Calorie Burn Estimator MCP server provides a precise way to calculate calories burned during physical activities. By using the Metabolic Equivalent of Task (MET) principle, it calculates energy expenditure based on your body weight and the duration of the exercise. You can use `search_activities` to find specific exercises in our database of over 80 activities, `estimate_calories_burned` to get exact calorie counts, and `classify_activity_intensity` to understand the physiological effort level of an activity.


## Available Tools
- **classify_activity_intensity**: Classify the intensity of an activity
- **estimate_calories_burned**: Estimate calories burned during an activity
- **search_activities**: Search for physical activities and their MET values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calorie Burn Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories do I burn if I run for 30 minutes at a weight of 70kg?"

**🤖 AI Agent:**
> Running (assuming a MET of 9.8) for 30 minutes at 70kg burns approximately 228.67 calories.

---

**👤 You:**
> "Find me some low intensity activities."

**🤖 AI Agent:**
> Some low intensity activities include walking, stretching, and light yoga.

---

**👤 You:**
> "What is the intensity level of an activity with a MET value of 7?"

**🤖 AI Agent:**
> An activity with a MET value of 7 is classified as Moderate Intensity.


## ❓ FAQ

**Q: How does the calorie estimation work?**
The calculation uses the MET (Metabolic Equivalent of Task) value for the activity, multiplied by your weight in kilograms and the duration in hours.

**Q: Where do the activity MET values come from?**
The server uses a hardcoded, reliable registry of over 80 physical activities with established metabolic intensities.

**Q: Can I search for specific exercises?**
Yes, you can use the `search_activities` tool to browse the full list or filter by keyword.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calorie-burn-estimator](https://vinkius.com/mcp/calorie-burn-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calorie Burn Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calorie-burn-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calorie Burn Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calorie-burn-estimator": {
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
