# Cryotherapy Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cryotherapy-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized whole-body cryotherapy session planning and safety assessment.

## Description
This MCP server provides specialized tools for planning whole-body cryotherapy (WBC) sessions. It helps users determine optimal exposure duration and frequency based on their experience level and specific goals like recovery or performance. Use `get_session_plan` for a complete prescription, `check_safety_eligibility` to identify contraindications, `get_goal_optimization` to refine session intensity, and `calculate_acclimatization_schedule` to help novice users safely build cold tolerance.


## Available Tools (4)
- **check_safety_eligibility**: Evaluates if a user is safe to undergo cryotherapy based on their health profile
- **calculate_acclimatization_schedule**: Creates a progressive ramp-up plan for new users to build cold tolerance
- **get_goal_optimization**: Provides guidance on how to adjust session parameters to better meet specific user objectives
- **get_session_plan**: Generates a complete, personalized cryotherapy session prescription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cryotherapy Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a novice looking for muscle recovery. What is my session plan for -120°C?"

**🤖 AI Agent:**
> For a novice at -120°C focusing on recovery, your recommended duration is 90 seconds, with a frequency of 3 sessions per week. Primary benefits include reduced muscle soreness and improved circulation.

---

**👤 You:**
> "Is it safe for someone with hypertension to use a -140°C chamber?"

**🤖 AI Agent:**
> Based on the health profile provided, cryotherapy at -140°C is not recommended due to the risk of increased blood pressure. Please consult a medical professional.

---

**👤 You:**
> "Create a ramp-up plan for a new user wanting to reach -150°C."

**🤖 AI Agent:**
> Your acclimatization plan will take 4 weeks. You will start with a maximum initial duration of 60 seconds at milder temperatures, gradually increasing intensity each week until you reach the target of -150°C.


## ❓ FAQ

**Q: How do I know if I am safe for cryotherapy?**
You can use the `check_safety_eligibility` tool to evaluate your health profile against intended chamber temperatures to identify potential contraindications.

**Q: Can I plan a session for a beginner?**
Yes, the `calculate_acclimatization_schedule` tool is specifically designed to create a progressive ramp-up plan for novice users.

**Q: How can I optimize my sessions for muscle recovery?**
You can use `get_goal_optimization` to receive guidance on adjusting session intensity and frequency to better meet your recovery objectives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cryotherapy-session-planner](https://vinkius.com/en/ai-agent-connect/cryotherapy-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cryotherapy Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cryotherapy-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cryotherapy Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cryotherapy-session-planner": {
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
