# Mechanical Drop Set Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mechanical-drop-set-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design progressive resistance training sequences using mechanical advantage transitions.

## Description
This MCP server provides specialized tools to design mechanical drop sets, a training technique that maximizes metabolic stress by transitioning through exercise variations of decreasing mechanical advantage. Use `plan_drop_set` to generate a complete sequence of variations, `get_exercise_progression` to view available leverage transitions, and `calculate_stress_profile` to estimate the physiological impact of your sets. It is designed to help athletes maintain high tension while moving from stronger to weaker leverage positions.


## Available Tools (4)
- **calculate_stress_profile**: Estimates the physiological impact of a completed or planned set
- **plan_drop_set**: Generates a complete, sequenced drop set plan based on a user's target intensity and desired volume
- **validate_variation_transition**: Verifies if a specific transition between two exercises is valid for a mechanical drop set
- **get_exercise_progression**: Retrieves the ordered list of variations available for a specific exercise to help users understand leverage transitions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mechanical Drop Set Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 2-drop set for a Bench Press starting with the wide-grip variation for 10 reps."

**🤖 AI Agent:**
> Your drop set plan is: 1. Wide-grip Bench Press: 10 reps, 2. Standard Bench Press: 8 reps, 3. Narrow-grip Bench Press: 6 reps.

---

**👤 You:**
> "What are the available variations for the Squat exercise?"

**🤖 AI Agent:**
> The available variations for Squat are: High Advantage (Back Squat), Mid Advantage (Front Squat), and Low Advantage (Goblet Squat).

---

**👤 You:**
> "Calculate the stress profile for a set of 12, 10, and 8 reps with leverage factors of 1.0, 0.8, and 0.6."

**🤖 AI Agent:**
> The calculated metabolic stress score is 24.0 and the tension persistence score is 12.0.


## ❓ FAQ

**Q: What is a mechanical drop set?**
A mechanical drop set is a technique where you transition to an easier variation of an exercise to continue training with the same weight, maximizing metabolic stress.

**Q: How do I generate a training plan?**
You can use the `plan_drop_set` tool by providing the exercise ID, starting variation, target repetitions, and the number of drops you want to perform.

**Q: Can I check if a transition is valid?**
Yes, use the `validate_variation_transition` tool to verify if moving from one variation to another follows the required mechanical advantage rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mechanical-drop-set-planner](https://vinkius.com/en/ai-agent-connect/mechanical-drop-set-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mechanical Drop Set Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mechanical-drop-set-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mechanical Drop Set Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mechanical-drop-set-planner": {
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
