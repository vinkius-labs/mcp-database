# Warm-up Set Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/warm-up-set-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates structured warm-up progressions for strength athletes.

## Description
This MCP server provides specialized tools for strength athletes to determine optimal preparatory sets. By using `calculate_warmup_routine`, athletes receive a structured sequence of weight, repetitions, and rest intervals tailored to their specific profile. The service accounts for exercise complexity via `get_exercise_complexity_factor`, adjusts for physiological safety using `get_safety_modifier`, and scales intensity based on training maturity with `get_experience_scaling`.


## Available Tools (4)
- **calculate_warmup_routine**: Generates a complete, structured sequence of warm-up sets for a specific lift
- **get_exercise_complexity_factor**: Determines the scale of the warm-up required based on the lift type
- **get_experience_scaling**: Adjusts the warm-up intensity based on how much training experience the user has
- **get_safety_modifier**: Calculates a physiological adjustment factor based on age and injury status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Warm-up Set Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a warm-up routine for a 30-year-old intermediate lifter doing a compound squat with a working weight of 100kg and no injury history."

**🤖 AI Agent:**
> Set 1: 40kg x 10 reps, 60s rest. Set 2: 60kg x 6 reps, 60s rest. Set 3: 80kg x 3 reps, 90s rest.

---

**👤 You:**
> "I am a 55-year-old novice lifter. Calculate a warm-up for a 50kg isolation bicep curl."

**🤖 AI Agent:**
> Set 1: 20kg x 12 reps, 45s rest. Set 2: 30kg x 8 reps, 45s rest.

---

**👤 You:**
> "Provide a warm-up for an advanced lifter doing a 150kg deadlift, age 25, with a recent lower back injury."

**🤖 AI Agent:**
> Set 1: 45kg x 12 reps, 60s rest. Set 2: 75kg x 8 reps, 60s rest. Set 3: 105kg x 4 reps, 120s rest. Set 4: 125kg x 2 reps, 120s rest.


## ❓ FAQ

**Q: How does the tool account for injury history?**
The `get_safety_modifier` tool calculates a physiological adjustment that reduces weight increments and increases volume buffers to prioritize joint health and tissue temperature.

**Q: Can I use this for compound lifts like Squats?**
Yes, `calculate_warmup_routine` uses the `get_exercise_complexity_factor` to ensure compound lifts receive more extensive warm-up progressions than isolation movements.

**Q: Does experience level affect the warm-up?**
Yes, the `get_experience_scaling` tool adjusts the intensity, allowing advanced lifters to use higher-intensity sets closer to their working weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/warm-up-set-calculator](https://vinkius.com/en/ai-agent-connect/warm-up-set-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Warm-up Set Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `warm-up-set-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Warm-up Set Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "warm-up-set-calculator": {
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
