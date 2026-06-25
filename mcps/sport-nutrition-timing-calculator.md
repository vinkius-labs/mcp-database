# Sport Nutrition Timing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sport-nutrition-timing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise carbohydrate and protein timing for pre-, intra-, and post-workout nutrition based on training intensity.

## Description
Optimize your athletic performance with precision nutrient timing. This MCP server provides a scientific approach to managing macronutrient intake around your training sessions. By analyzing your training start time, duration, and intensity level (LOW, MEDIUM, or HIGH), the calculator determines exactly when you should consume carbohydrates and proteins to maximize energy availability and muscle recovery.

Key features include:
- **Pre-Workout Planning**: Identifies two critical windows--one 3-4 hours before training for sustained energy, and another 3-60 minutes before for rapid glucose availability.
- **Intra-Workout Support**: For sessions exceeding 60 minutes, it calculates the necessary carbohydrate grams per hour to prevent glycogen depletion.
- **Post-Workout Recovery**: Defines the anabolic window (30-60 minutes post-training) with specific protein and carbohydrate targets to facilitate muscle protein synthesis.

Use `calculate_pre_workout_needs` for early preparation, `calculate_intra_workout_needs` for long sessions, and integrate these into your training routine via Vinkius Edge.


## Available Tools (2)
- **calculate_intra_workout_needs**: Calculate carbohydrate replenishment needs for training
- **calculate_pre_workout_needs**: Calculate macronutrient targets and meal timing for pre-workout


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sport Nutrition Timing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a high-intensity training session starting at 2023-10-27T14:00:00Z. What should my pre-workout nutrition look like?"

**🤖 AI Agent:**
> For your high-intensity session, you should follow two windows: 3-4 hours before (Window 1) and 30-60 minutes before (Window 2). Your targets will include specific carbohydrate and protein grams to support the metabolic demand. Suggested foods include oats for Window 1 and bananas or rice cakes for Window 2.

---

**👤 You:**
> "I am training for 90 minutes at medium intensity. Do I need intra-workout nutrition?"

**🤖 AI Agent:**
> Yes, since your session is longer than 60 minutes, you require intra-workout nutrition. You should aim for a carbohydrate range of approximately 30-6    grams per hour to maintain energy levels.

---

**👤 You:**
> "What are the macronutrient targets for a low-intensity session lasting 45 minutes?"

**🤖 AI Agent:**
> For a 45-minute low-intensity session, intra-workout nutrition is not required. Your focus should be on the pre-workout windows to ensure adequate energy availability without excessive intake.


## ❓ FAQ

**Q: How does intensity level affect the results?**
The intensity level (LOW, MEDIUM, or HIGH) directly scales your carbohydrate and protein requirements. Higher intensity sessions trigger higher macronutrient targets to compensate for greater metabolic demand.

**Q: When should I use the intra-workout tool?**
You should use `calculate_intra_workout_needs` only if your training session duration is expected to exceed 60 minutes. For shorter sessions, intra-workout nutrition is typically not required.

**Q: Does this tool provide food suggestions?**
Yes, the `calculate_pre_workout_needs` tool provides specific examples of foods suitable for both the early and late pre-workout windows based on your training intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sport-nutrition-timing-calculator](https://vinkius.com/mcp/sport-nutrition-timing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sport Nutrition Timing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sport-nutrition-timing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sport Nutrition Timing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sport-nutrition-timing-calculator": {
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
