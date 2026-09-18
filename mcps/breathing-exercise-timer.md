# Breathing Exercise Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/breathing-exercise-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured breathing patterns and physiological insights.

## Description
This MCP server provides tools to create structured breathing exercise schedules. Users can generate specific patterns for techniques like Box Breathing, 4-7-8, or the Wim Hof Method. The server calculates session metrics such as breaths per minute and provides physiological insights into how each technique affects the nervous system. It also includes safety modifications for beginners using `get_difficulty_modifications` to ensure comfort during practice.


## Available Tools (4)
- **calculate_session_stats**: Validates and summarizes the metrics of a generated breathing pattern
- **get_breathing_pattern**: Generates a complete breathing schedule based on a specific technique and time goal
- **get_difficulty_modifications**: Provides guidance on how to adjust a technique for beginners
- **get_physiological_impact**: Describes the biological benefits and intended effects of a specific technique


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breathing Exercise Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 5-minute Box Breathing session for me."

**🤖 AI Agent:**
> Your 5-minute Box Breathing session is ready. It consists of 15 cycles with a pattern of 4s inhale, 4s hold, 4s exhale, and 4s hold. Your rate is 3.75 breaths per minute.

---

**👤 You:**
> "What are the benefits of the 4-7-8 technique?"

**🤖 AI Agent:**
> The 4-7-8 technique is primarily used for Stress Reduction and targets Parasympathetic Activation with a Low intensity level.

---

**👤 You:**
> "I am a beginner at Wim Hof breathing. How should I adjust?"

**🤖 AI Agent:**
> For beginners, it is recommended to use reduced hold times. Focus on nasal breathing to ensure safety and comfort.


## ❓ FAQ

**Q: What breathing techniques are supported?**
The server supports Box Breathing, 4-7-8, and the Wim Hof Method through the `get_breathing_pattern` tool.

**Q: Can I adjust the exercises for beginners?**
Yes, you can use `get_difficulty_modifications` to receive suggested hold times and tips for safer practice.

**Q: How do I know the physiological effects of a technique?**
You can use `get_physiological_impact` to understand the primary effects and target nervous system state for any technique.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/breathing-exercise-timer](https://vinkius.com/en/ai-agent-connect/breathing-exercise-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breathing Exercise Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breathing-exercise-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breathing Exercise Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breathing-exercise-timer": {
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
