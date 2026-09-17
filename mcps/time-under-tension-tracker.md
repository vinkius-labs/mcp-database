# Time Under Tension Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/time-under-tension-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and optimize training stimulus by tracking muscle contraction duration.

## Description
This MCP server provides specialized tools for strength athletes to measure Time Under Tension (TUT). By inputting repetition tempo (eccentric, pause, and concentric phases) and rep counts, users can use `calculate_set_tut` to find total duration, `get_phase_distribution` to see time allocation, and `analyze_training_goal` to determine if a set favors hypertrophy or strength. It also provides recovery guidance via `recommend_rest_period` based on training objectives and intensity.


## Available Tools (4)
- **analyze_training_goal**: Categorizes the set's effectiveness for specific physiological outcomes
- **calculate_set_tut**: Determines the total duration of a single set based on the tempo and repetition count
- **get_phase_distribution**: Provides a breakdown of how time was distributed across the movement phases
- **recommend_rest_period**: Suggests an appropriate recovery duration between sets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time Under Tension Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I did 10 reps with a 3s eccentric, 1s pause, and 1s concentric tempo. What was my total TUT?"

**🤖 AI Agent:**
> Your total time under tension for that set was 50 seconds.

---

**👤 You:**
> "Is a set with 60 seconds of TUT good for hypertrophy?"

**🤖 AI Agent:**
> Yes, a 60-second TUT is generally well-suited for hypertrophy as it provides sufficient metabolic stress.

---

**👤 You:**
> "I'm training for strength at high intensity. How long should I rest?"

**🤖 AI Agent:**
> For high-intensity strength training, a rest period of 180 seconds is recommended to allow for full ATP replenishment.


## ❓ FAQ

**Q: How do I calculate my total time under tension?**
You can use the `calculate_set_tut` tool by providing the number of repetitions and the duration of the eccentric, pause, and concentric phases.

**Q: Can this tool help with muscle growth?**
Yes, the `analyze_training_goal` tool evaluates your TUT to determine its suitability for hypertrophy or strength training.

**Q: How much rest should I take between sets?**
The `recommend_rest_period` tool suggests recovery durations based on your specific training goal and the intensity of the set.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/time-under-tension-tracker](https://vinkius.com/en/ai-agent-connect/time-under-tension-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Time Under Tension Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `time-under-tension-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Time Under Tension Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "time-under-tension-tracker": {
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
