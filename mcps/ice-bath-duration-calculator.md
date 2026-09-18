# Ice Bath Duration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ice-bath-duration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates safe ice bath durations and progression plans based on your physiological profile.

## Description
This MCP server provides specialized tools for safe cold water immersion. Use `get_safe_duration` to determine optimal immersion times based on water temperature, body fat, and cold tolerance. You can use `evaluate_hypothermia_risk` to assess safety levels, `calculate_progression_plan` to build a roadmap for increasing cold intensity, and `get_goal_specific_guidance` for tailored recovery or mental resilience tips.


## Available Tools (4)
- **calculate_progression_plan**: Generates a roadmap for users to gradually increase their cold exposure intensity
- **evaluate_hypothermia_risk**: Assesses the danger level of a planned or completed ice bath
- **get_goal_specific_guidance**: Provides qualitative advice and frequency recommendations tailored to the user's intent
- **get_safe_duration**: Determines the optimal amount of time a user should stay in the water based on their specific profile and goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ice Bath Duration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long should I stay in 5°C water if I have 15% body fat and low cold tolerance for muscle recovery?"

**🤖 AI Agent:**
> Based on your profile, the recommended safe duration is 2 minutes. You should perform this session 2 times per week.

---

**👤 You:**
> "Is it dangerous to stay in 2°C water for 10 minutes with 10% body fat?"

**🤖 AI Agent:**
> High Risk. Staying in 2°C water for 10 minutes with 10% body fat poses a significant hypothermia risk.

---

**👤 You:**
> "I am currently comfortable at 15°C and want to reach 5°C. What is my plan?"

**🤖 AI Agent:**
> Your progression plan includes 4 steps over 4 weeks, gradually decreasing the temperature by 2.5°C each week.


## ❓ FAQ

**Q: How do I know if my ice bath is safe?**
You can use the `evaluate_hypothermia_risk` tool to assess the danger level based on your planned duration, water temperature, and body fat percentage.

**Q: Can I use this for muscle recovery after training?**
Yes. By setting the `isPostWorkout` parameter to true in `get_safe_duration`, the tool optimizes the duration for physiological recovery.

**Q: How can I gradually get used to colder water?**
The `calculate_progression_plan` tool generates a step-by-step roadmap to help you reach your target temperature safely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ice-bath-duration-calculator](https://vinkius.com/en/ai-agent-connect/ice-bath-duration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ice Bath Duration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ice-bath-duration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ice Bath Duration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ice-bath-duration-calculator": {
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
