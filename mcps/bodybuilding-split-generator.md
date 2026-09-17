# Bodybuilding Split Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bodybuilding-split-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates personalized bodybuilding split routines based on training frequency and muscle priorities.

## Description
This MCP server provides a complete suite of tools to design hypertrophy-focused training programs. Use `get_split_structure` to organize your weekly schedule, `calculate_muscle_volume` to determine set counts based on your muscle priorities, and `generate_exercise_selection` to pick specific movements. Finally, use `verify_recovery_protocol` to ensure your training days allow for optimal muscle protein synthesis and recovery.


## Available Tools (4)
- **calculate_muscle_volume**: Determine the specific workload assigned to each muscle group
- **generate_exercise_selection**: Select specific exercises for each muscle group
- **verify_recovery_protocol**: Ensure the generated split allows for sufficient rest
- **get_split_structure**: Determine the foundational organization of the training week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bodybuilding Split Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 4-day split for an intermediate lifter focusing on Chest and Back."

**🤖 AI Agent:**
> Your 4-day intermediate split is organized as: Monday: Chest/Back, Tuesday: Legs/Core, Thursday: Chest/Back, Friday: Shoulders/Arms. Total weekly sets for Chest: 12, Back: 12.

---

**👤 You:**
> "I am a beginner training 3 days a week. What should my split look like?"

**🤖 AI Agent:**
> For a 3-day beginner split, a Full Body routine is recommended: Monday, Wednesday, and Friday. This ensures high frequency for foundational movements.

---

**👤 You:**
> "Check if my 5-day advanced split is safe for recovery."

**🤖 AI Agent:**
> The schedule is recoverable. Your rest days are set for Wednesday and Sunday, providing sufficient time between high-volume sessions.


## ❓ FAQ

**Q: How do I create a full workout plan?**
You should first call `get_split_structure` to define your days, then `calculate_muscle_volume` for set counts, and finally `generate_exercise_selection` to get the specific exercises.

**Q: Can I prioritize specific muscles?**
Yes, use the `calculate_muscle_volume` tool and provide your preferred muscle groups in the `musclePriorities` array to increase their weekly volume.

**Q: How does the tool handle recovery?**
The `verify_recovery_protocol` tool checks your schedule against physiological principles to ensure you have enough rest between training the same muscle groups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bodybuilding-split-generator](https://vinkius.com/en/ai-agent-connect/bodybuilding-split-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bodybuilding Split Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bodybuilding-split-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bodybuilding Split Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bodybuilding-split-generator": {
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
