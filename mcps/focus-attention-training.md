# Focus Attention Training MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/focus-attention-training)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Mental training system for surfers to optimize performance through directed attention.

## Description
This MCP server provides a specialized psychological framework for surfers to manage attention shifts. By using tools like `generate_focus_drills` and `create_attention_cues`, surfers can transition from internal focus (body mechanics) to external focus (environmental scanning) to improve motor learning and flow. The system also allows users to `build_practice_protocol` for both controlled and chaotic ocean environments and `assess_attention_capacity` to ensure readiness for high-complexity performance goals.


## Available Tools (4)
- **assess_attention_capacity**: Analyzes if the current focus level is sufficient for the stated goals
- **build_practice_protocol**: Provide drills as a JSON string.

Assembles a structured training routine combining drills and cues into a timed session
- **create_attention_cues**: Generates immediate mental triggers to help the user combat specific distractions
- **generate_focus_drills**: Provides specific mental exercises to strengthen the user's ability to sustain focus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus Attention Training** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to improve my barrel riding. My current focus level is 70. Give me some drills for external focus."

**🤖 AI Agent:**
> Here are your external focus drills for barrel riding: 1. Wave Face Scanning (5 mins) - Observe the lip movement. 2. Horizon Stabilization (5 mins) - Keep eyes fixed on the distant swell.

---

**👤 You:**
> "I'm feeling distracted by the crowd in the water. Help me with a cue."

**🤖 AI Agent:**
> To counter environmental distractions, use this external cue: 'Watch the lip'.

---

**👤 You:**
> "Is my focus level of 50 enough for a goal complexity of 8?"

**🤖 AI Agent:**
> No, your readiness score is low. We recommend increasing your focus drills or lowering the goal complexity to manage the high risk level.


## ❓ FAQ

**Q: How do I use the focus drills?**
You can use the `generate_focus_drills` tool by providing your current focus level, your primary surfing goal, and whether you want to focus on internal or external cues.

**Q: Can I prepare for ocean conditions?**
Yes, the `build_practice_protocol` tool allows you to design routines specifically for 'chaotic' environments like the open ocean.

**Q: What is the difference between internal and external focus?**
External focus directs attention to the environment or movement effects, while internal focus directs attention to body mechanics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/focus-attention-training](https://vinkius.com/en/ai-agent-connect/focus-attention-training)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus Attention Training** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `focus-attention-training` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus Attention Training** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-attention-training": {
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
