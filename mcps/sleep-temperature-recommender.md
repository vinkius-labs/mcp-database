# Sleep Temperature Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-temperature-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates optimal bedroom temperatures based on personal preference, bedding, and health.

## Description
This MCP server provides specialized advisory tools to optimize sleep environments. It uses thermal comfort research to determine the ideal ambient temperature range via `get_optimal_temperature_range`. Users can receive specific guidance on adjusting their setup using `get_bedding_adjustment_advice`, align their environment with biological rhythms through `get_circadian_alignment_plan`, and ensure physiological safety with `validate_thermal_safety`.


## Available Tools (4)
- **get_bedding_adjustment_advice**: Provide guidance on adjusting bedding to reach a target temperature
- **get_circadian_alignment_plan**: Align ambient temperature recommendations with the user's biological sleep-wake cycle
- **get_optimal_temperature_range**: Determine the ideal ambient temperature range for a user's specific sleep environment
- **validate_thermal_safety**: Check if a proposed temperature setup poses a risk to a user with specific health conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Temperature Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I prefer a cool room, I'm using light bedding and no extra clothing, and it is currently winter. What temperature should my room be?"

**🤖 AI Agent:**
> Your recommended temperature range is 18°C to 21°C for a comfortable, cool sleep environment.

---

**👤 You:**
> "I want my room to be 22°C, but I am currently using heavy bedding. What should I do?"

**🤖 AI Agent:**
> You should decrease insulation by switching to medium or light bedding to reach your target temperature.

---

**👤 You:**
> "I need to wake up at 07:00. My recommended range is 19-22°C. What should my temperature settings be?"

**🤖 AI Agent:**
> Set your temperature to 19°C for sleep onset and increase it to 22°C in the morning to support your wake-up time.


## ❓ FAQ

**Q: How does the tool account for my health conditions?**
The `validate_thermal_safety` tool specifically checks if a proposed temperature poses risks based on your medical history, while `get_optimal_temperature_range` adjusts the recommended range to accommodate thermoregulation needs.

**Q: Can I adjust my bedding instead of the room temperature?**
Yes, you can use `get_bedding_adjustment_advice` to receive specific recommendations on whether to increase or decrease your bedding insulation to reach your target temperature.

**Q: How does this help with my sleep schedule?**
The `get_circadian_alignment_plan` tool provides a temperature strategy that supports your natural biological rhythms, suggesting specific settings for sleep onset and waking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-temperature-recommender](https://vinkius.com/en/ai-agent-connect/sleep-temperature-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Temperature Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-temperature-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Temperature Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-temperature-recommender": {
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
