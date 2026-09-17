# Accessory Exercise Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessory-exercise-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recommends supplemental exercises, volume, and sequencing based on your primary lifts and weaknesses.

## Description
This MCP server acts as a specialized strength training decision engine. It connects your AI assistant to advanced periodization logic to help you overcome plateaus. By analyzing your primary lift, specific muscle weaknesses, and available gym equipment, it provides precise exercise recommendations, set/rep schemes, and optimal workout sequencing. You can use `get_accessory_recommendations` to find the right movements, `get_workout_sequence` to organize your session, and `get_progression_plan` to manage long-term strength gains.


## Available Tools (4)
- **get_accessory_recommendations**: Suggests specific exercises and volume parameters to address a user's training needs
- **get_progression_plan**: Provides a strategy for increasing the load or difficulty of the chosen exercises over subsequent training sessions
- **validate_equipment_feasibility**: Checks if a specific list of exercises can actually be performed with the user's current equipment
- **get_workout_sequence**: Determines the optimal order for the recommended accessory exercises within a single workout session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessory Exercise Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am focusing on the Back Squat but my core is a weak point. I only have a barbell. What should I do for my hypertrophy phase?"

**🤖 AI Agent:**
> For your hypertrophy phase focusing on core stability for the Back Squat using a barbell, I recommend performing Barbell Rollouts for 3 sets of 12 repetitions.

---

**👤 You:**
> "What is the best order for these exercises: Bench Press, Tricep Extensions, and Pushups?"

**🤖 AI Agent:**
> The optimal sequence for your workout is Bench Press, followed by Pushups, and finishing with Tricep Extensions.

---

**👤 You:**
> "I've been doing 3 sets of 10 reps of Dumbbell Lunges. How should I progress in my strength phase?"

**🤖 AI Agent:**
> To progress in your strength phase, you should increase the weight of the dumbbells once you can comfortably complete all 10 repetitions for all 3 sets.


## ❓ FAQ

**Q: How do I get exercise suggestions?**
You can ask your AI assistant to suggest exercises by providing your primary lift, weaknesses, and available equipment. The `get_accessory_recommendations` tool will then generate a tailored plan.

**Q: Can I use this if I only have dumbbells?**
Yes. When you specify your available equipment, the tool uses `validate_equipment_feasibility` to ensure all recommended exercises can be performed with what you have.

**Q: How does the progression work?**
The server provides specific instructions for increasing difficulty via `get_progression_plan`, adjusting weight or repetitions based on your current training phase like Hypertrophy or Strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessory-exercise-selector](https://vinkius.com/en/ai-agent-connect/accessory-exercise-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessory Exercise Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessory-exercise-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessory Exercise Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessory-exercise-selector": {
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
