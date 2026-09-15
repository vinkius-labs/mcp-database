# Strength Training Periodization for Surfers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/strength-training-periodization-for-surfers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Generate periodized strength programs tailored for surfers to peak for competitions.

## Description
This MCP server provides specialized periodization engines for surfers. It calculates training phases, volume/intensity progression, and recovery weeks based on competition schedules. Use `generate_training_plan` to build a full schedule, `evaluate_readiness` to check training load proximity to events, `get_movement_templates` for surf-specific exercises, and `calculate_deload_schedule` to manage recovery periods.


## Available Tools (4)
- **calculate_deload_schedule**: Determines exactly when recovery weeks should occur within a given timeframe
- **evaluate_readiness**: Determines if the athlete's current training load is appropriate given their proximity to a competition
- **generate_training_plan**: Creates a full periodized training schedule based on user profile and competition dates
- **get_movement_templates**: Retrieves a list of exercises categorized by their relevance to surfing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strength Training Periodization for Surfers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a training plan for a beginner surfer with a competition on 2025-06-01 focusing on explosive power."

**🤖 AI Agent:**
> Your periodized plan is ready. It includes a Preparatory phase for foundation, followed by Strength and Power phases, peaking just before your June 1st competition.

---

**👤 You:**
> "What exercises should I do for rotational stability?"

**🤖 AI Agent:**
> For rotational stability, you should focus on movements like Russian twists and medicine ball rotational throws.

---

**👤 You:**
> "Am I ready for my competition if I am in the Strength phase and the event is in 1 week?"

**🤖 AI Agent:**
> No, you should be in the Peaking phase. It is recommended to reduce intensity significantly to ensure you are fresh for the event.


## ❓ FAQ

**Q: How do I create a training plan for my next competition?**
You can use the `generate_training_plan` tool by providing your competition dates, current strength level, and your specific training goal.

**Q: Can I find exercises specific to surfing movements?**
Yes, the `get_movement_templates` tool provides exercises categorized by rotational, posterior chain, and explosive needs.

**Q: How does the tool handle recovery?**
The server uses `calculate_deload_schedule` to determine optimal recovery weeks to prevent overtraining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/strength-training-periodization-for-surfers](https://vinkius.com/en/ai-agent-connect/strength-training-periodization-for-surfers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strength Training Periodization for Surfers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strength-training-periodization-for-surfers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strength Training Periodization for Surfers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strength-training-periodization-for-surfers": {
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
