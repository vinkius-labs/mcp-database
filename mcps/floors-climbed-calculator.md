# Floors Climbed Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/floors-climbed-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Quantify the metabolic, distance, and cardiovascular impact of stair climbing.

## Description
This MCP server provides specialized tools to calculate the physiological impact of stair climbing. Use `calculate_stair_climbing_metrics` to determine calories burned and walking equivalence, `get_walking_equivalence_comparison` to compare stair climbing to horizontal walking, `estimate_cardiovascular_impact` to find your aerobic intensity, and `convert_floors_to_vertical_height` for vertical distance conversions.


## Available Tools (4)
- **calculate_stair_climbing_metrics**: Provides a comprehensive overview of the energy, distance, and health impact of a single climbing session
- **convert_floors_to_vertical_height**: A utility to validate and convert floor counts into total vertical distance
- **estimate_cardiovascular_impact**: Determines the intensity level of the exercise to help users understand the aerobic benefit
- **get_walking_equivalence_comparison**: Answers how much horizontal walking is required to match the specific caloric burn of a stair session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floors Climbed Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I climbed 10 floors, I weigh 75kg, each step is 0.18m high, and I climbed at 1.2 m/s. How many calories did I burn?"

**🤖 AI Agent:**
> You burned 42.5 calories during your 10-floor climb.

---

**👤 You:**
> "How much walking is equivalent to burning 50 calories on stairs?"

**🤖 AI Agent:**
> Burning 50 calories on stairs is equivalent to walking approximately 2.4 kilometers at a brisk pace.

---

**👤 You:**
> "What is the cardiovascular intensity of climbing at 1.5 m/s with 0.2m steps?"

**🤖 AI Agent:**
> At that speed and step height, your intensity category is Vigorous.


## ❓ FAQ

**Q: How does stair climbing compare to walking?**
Stair climbing is significantly more intense. You can use `get_walking_equivalence_comparison` to see how many kilometers of walking match your specific stair climbing session.

**Q: Does the tool account for descending stairs?**
Yes, `calculate_stair_climbing_metrics` allows you to specify if the session was ascent only or included descent, adjusting the metabolic cost accordingly.

**Q: Can I estimate my heart rate zone?**
Yes, by using `estimate_cardiovascular_impact`, you can determine your intensity category and estimated heart rate zone based on your climbing speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/floors-climbed-calculator](https://vinkius.com/en/ai-agent-connect/floors-climbed-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floors Climbed Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `floors-climbed-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floors Climbed Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floors-climbed-calculator": {
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
