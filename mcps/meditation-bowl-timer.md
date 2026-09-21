# Meditation Bowl Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meditation-bowl-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates precise striking and silence patterns for singing bowl meditation sessions.

## Description
This MCP server provides a precision scheduling engine for singing bowl practitioners. By analyzing bowl material and meditation intent, it calculates optimal striking patterns, sustain timings, and silence intervals. Use `get_session_plan` to generate a complete sequence of events, or `get_striking_cadence` to determine specific rhythmic intervals. It also includes `get_bowl_acoustics` to understand resonance properties and `validate_session_constraints` to ensure your requested session is physically viable.


## Available Tools (4)
- **get_bowl_acoustics**: Retrieves the specific sustain and decay characteristics based on the bowl material
- **get_session_plan**: Generates a complete, step-by-step sequence of strikes and silences for a meditation session
- **get_striking_cadence**: Determines the specific rhythm and frequency of strikes for a given goal
- **validate_session_constraints**: Checks if a requested session configuration is physically or logically viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meditation Bowl Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 10-minute relaxation session using a metal bowl."

**🤖 AI Agent:**
> Your 10-minute relaxation session for a metal bowl is ready. It will feature slow, rhythmic strikes with extended silence intervals to maximize the rich resonance of the metal.

---

**👤 You:**
> "I need a 5-minute focus session with a crystal bowl. What is the cadence?"

**🤖 AI Agent:**
> For a 5-minute focus session with a crystal bowl, the cadence will feature steady, frequent strikes with shorter silence intervals to maintain your cognitive presence.

---

**👤 You:**
> "What are the acoustic properties of a crystal bowl?"

**🤖 AI Agent:**
> Crystal bowls are characterized by a high purity of tone and a predictable, medium-duration resonance.


## ❓ FAQ

**Q: How do I generate a full session schedule?**
You can use the `get_session_plan` tool to receive a complete, step-by-step sequence of strikes and silences tailored to your bowl type and goal.

**Q: Can I use this for both metal and crystal bowls?**
Yes, the engine accounts for the different acoustic properties of both metal and crystal bowls to ensure accurate timing.

**Q: What happens if my session duration is too short?**
The `validate_session_constraints` tool will check your parameters and notify you if the requested duration is too short to accommodate the necessary strikes and sustain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meditation-bowl-timer](https://vinkius.com/en/ai-agent-connect/meditation-bowl-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meditation Bowl Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meditation-bowl-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meditation Bowl Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meditation-bowl-timer": {
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
