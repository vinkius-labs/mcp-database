# practice-repetition-total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/practice-repetition-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total training workload and volume distribution across exercise categories.

## Description
This MCP server provides tools for fitness trainers and athletes to track training intensity. It allows for calculating the total workload volume of a session using `calculate_session_total_reps`, identifying the most demanding movements with `get_highest_repetition_exercise`, and analyzing how volume is distributed across categories like Strength or Skill using `analyze_volume_distribution`. It helps in monitoring progress and managing training load effectively.


## Available Tools (4)
- **analyze_volume_distribution**: Provides a breakdown of how repetitions are distributed across different categories
- **calculate_session_total_reps**: Calculates the total number of repetitions performed in a complete training session
- **get_exercise_group_volume**: Answers how much work was done within a specific category of movement
- **get_highest_repetition_exercise**: Identifies which single exercise had the most repetitions performed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **practice-repetition-total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total volume for this session: [{'reps': 10}, {'reps': 20}, {'reps': 5}]?"

**🤖 AI Agent:**
> The total volume for your session is 35 repetitions.

---

**👤 You:**
> "Which exercise had the most reps: [{'name': 'Squat', 'reps': 12}, {'name': 'Pushup', 'reps': 25}]?"

**🤖 AI Agent:**
> The exercise with the most repetitions was Pushup with 25 reps.

---

**👤 You:**
> "Show me the volume distribution for: [{'reps': 10, 'category': 'Strength'}, {'reps': 5, 'category': 'Skill'}, {'reps': 15, 'category': 'Strength'}]"

**🤖 AI Agent:**
> The volume distribution is: Strength: 25, Skill: 5.


## ❓ FAQ

**Q: How do I calculate the total repetitions for my workout?**
You can use the `calculate_session_total_reps` tool by providing a list of your exercises and their respective repetition counts.

**Q: Can I see how much volume I did in a specific category?**
Yes, the `get_exercise_group_volume` tool allows you to filter repetitions by a specific category like 'Strength' or 'Skill'.

**Q: How do I find my most intense exercise?**
Use the `get_highest_repetition_exercise` tool to identify which single movement had the highest number of repetitions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/practice-repetition-total](https://vinkius.com/en/ai-agent-connect/practice-repetition-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **practice-repetition-total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `practice-repetition-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **practice-repetition-total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "practice-repetition-total": {
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
