# Artist Critique Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/artist-critique-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Facilitate professional art critiques with structured agendas, reviewer briefings, and actionable follow-up plans.

## Description
This MCP server provides a complete facilitation engine for professional art critique sessions. It helps artists transform their requirements into structured workflows by providing tools to `generate_critique_agenda` for timed schedules, `prepare_reviewer_briefing` to set clear boundaries and questions for critics, `sequence_work_presentation` to organize the flow of artworks, `format_response_capture` to create tailored feedback templates, and `plan_next_actions` to turn feedback into concrete artistic tasks. It ensures that feedback remains within the creator's defined boundaries while maximizing the utility of the session for the intended follow-up goal.


## Available Tools (5)
- **format_response_capture**: Provides a template for recording the feedback received during the session
- **generate_critique_agenda**: Creates a timed schedule for the session
- **plan_next_actions**: Translates the feedback and goals into a concrete plan for the artist
- **prepare_reviewer_briefing**: Generates a guidance document for the invited reviewers
- **sequence_work_presentation**: Determines the most effective order in which to view and discuss the works


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Artist Critique Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 3 paintings to discuss in a 45-minute session. I want a conversational style. Can you make an agenda?"

**🤖 AI Agent:**
> Here is your 45-minute conversational agenda: 1. Introduction (5 mins), 2. Painting A Discussion (12 mins), 3. Painting B Discussion (12 mins), 4. Painting C Discussion (12 mins), 5. Wrap-up (4 mins).

---

**👤 You:**
> "Help me prepare my reviewers. I want to ask about color usage, but I do NOT want any feedback on my composition."

**🤖 AI Agent:**
> Reviewer Briefing: Focus on color usage. WARNING: Do not provide feedback on composition.

---

**👤 You:**
> "I received feedback that my lighting is too harsh and my textures need more detail. My goal is technical improvement. What should I do next?"

**🤖 AI Agent:**
> Action Plan: 1. Practice soft-light blending techniques. 2. Study high-detail texture studies. 3. Re-evaluate lighting setups for upcoming works.


## ❓ FAQ

**Q: How does this tool help manage feedback boundaries?**
The `prepare_reviewer_briefing` tool allows you to explicitly list topics to avoid, ensuring reviewers respect your defined constraints.

**Q: Can I customize the session timing?**
Yes, using `generate_critique_agenda`, you can specify the total duration and the number of works to create a balanced schedule.

**Q: How do I turn feedback into actual work?**
The `plan_next_actions` tool analyzes your captured feedback and translates it into specific, measurable tasks oriented toward your goal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/artist-critique-session-planner](https://vinkius.com/en/ai-agent-connect/artist-critique-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Artist Critique Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `artist-critique-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Artist Critique Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "artist-critique-session-planner": {
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
