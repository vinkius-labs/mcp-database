# Coaching Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coaching-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured surf coaching session plans, drill progressions, and feedback strategies.

## Description
This MCP server connects AI agents to professional surf coaching methodologies. It allows for the generation of complete session plans using `get_session_plan`, checking the safety and effectiveness of specific exercises with `evaluate_drill_feasibility`, determining the best timing for coaching via `calculate_feedback_cadence`, and mapping out skill development through `get_progression_path`.


## Available Tools (4)
- **calculate_feedback_cadence**: Determines the optimal timing and frequency of coaching feedback
- **evaluate_drill_feasibility**: Determines if a specific drill is appropriate given the current environmental conditions
- **get_progression_path**: Provides a sequence of drills to help a student reach a specific goal
- **get_session_plan**: Generates a complete, structured plan for a single surf coaching session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coaching Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a session plan for an Intermediate surfer aiming to improve turns in Good wave conditions with a Moderate crowd."

**🤖 AI Agent:**
> The session plan includes a 10-minute warm-up, a 30-minute technical execution phase focusing on carving turns, and a 10-minute review. Recommended drills include 'Bottom Turn Precision' and 'Top Turn Control'.

---

**👤 You:**
> "Is a high-performance carve feasible in Heavy waves with an Extremely Crowded lineup?"

**🤖 AI Agent:**
> No, the high-performance carve is not feasible due to the high collision risk in crowded conditions and the intensity of the waves.

---

**👤 You:**
> "What is the next step for a Beginner wanting to improve their pop-up?"

**🤖 AI Agent:**
> The next step in the progression is 'Stable Pop-up Mechanics' to build the necessary foundation for wave riding.


## ❓ FAQ

**Q: How does the session plan adapt to different surf conditions?**
The `get_session_plan` tool automatically adjusts the session structure based on wave quality and crowd density to ensure safety and optimal learning.

**Q: Can I check if a specific maneuver is safe for a beginner?**
Yes, you can use `evaluate_drill_feasibility` to determine if a drill is appropriate for the current wave quality and crowd factor.

**Q: How is feedback timing determined?**
The `calculate_feedback_cadence` tool analyzes the student's proficiency and the wave conditions to recommend the most effective frequency and timing for coaching.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coaching-session-planner](https://vinkius.com/en/ai-agent-connect/coaching-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coaching Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coaching-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coaching Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coaching-session-planner": {
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
