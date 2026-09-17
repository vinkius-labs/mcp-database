# Tempo Prescription MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tempo-prescription)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Get precise lifting tempo sequences based on your training goals and experience.

## Description
This MCP server provides specialized lifting tempo programming. By using tools like `get_tempo_prescription`, you can receive exact timing for the eccentric, pause, and concentric phases of any exercise. Whether you are training for strength, hypertrophy, or control, the server calculates the optimal repetition duration to match your experience level.


## Available Tools (4)
- **get_exercise_tempo_range**: Provides the standard tempo duration boundaries for a specific exercise
- **get_tempo_guidelines**: Provides general tempo principles and recommended ranges for a specific training goal
- **get_tempo_prescription**: Prescribes a specific lifting tempo sequence based on exercise, goal, and experience
- **validate_tempo_sequence**: Validates if a specific tempo sequence is appropriate for the user's goal and experience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tempo Prescription** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What tempo should I use for a Bench Press if I want hypertrophy and I am an intermediate lifter?"

**🤖 AI Agent:**
> For an intermediate lifter focused on hypertrophy, a recommended tempo for Bench Press is 3 seconds eccentric, 1 second pause at the bottom, and 1 second concentric.

---

**👤 You:**
> "Give me a strength tempo for Squats for a beginner."

**🤖 AI Agent:**
> A beginner strength tempo for Squats is 3 seconds eccentric, 2 seconds pause at the bottom, and 1 second concentric.

---

**👤 You:**
> "What are the general tempo principles for hypertrophy?"

**🤖 AI Agent:**
> Hypertrophy training focuses on increasing Time Under Tension (TUT) through longer eccentric phases and controlled pauses.


## ❓ FAQ

**Q: How do I get a specific tempo for my squat?**
You can use the `get_tempo_prescription` tool by providing 'Squat' as the exercise, along with your specific goal and experience level.

**Q: Can I check if my custom tempo is safe?**
Yes, use the `validate_tempo_sequence` tool to verify if your chosen timing is appropriate for your training profile.

**Q: What training goals are supported?**
The server supports strength, hypertrophy, and control objectives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tempo-prescription](https://vinkius.com/en/ai-agent-connect/tempo-prescription)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tempo Prescription** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tempo-prescription` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tempo Prescription** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tempo-prescription": {
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
