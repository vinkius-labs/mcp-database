# Creative Project Retrospective Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-project-retrospective-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform raw post-project data into structured retrospective outputs and strategic creative directions.

## Description
This MCP server provides a suite of strategic tools to help creators and teams process project completions. By analyzing intended outcomes, participant reflections, and audience responses, it generates actionable insights. Use `generate_retrospective_agenda` to structure review meetings, `derive_decision_matrix` to identify what to keep or stop, `compile_documentation_summary` for archival, `formulate_next_direction` for future planning, and `execute_acknowledgement_actions` to recognize contributors.


## Available Tools (5)
- **execute_acknowledgement_actions**: Identifies specific people or entities that require recognition based on the project's decisions and outcomes
- **compile_documentation_summary**: Aggregates all project data into a concise summary for archival and rights management
- **derive_decision_matrix**: Synthesizes participant reflections and decisions into a "Keep, Change, Stop" actionable list
- **formulate_next_direction**: Produces a strategic brief for the subsequent creative endeavor
- **generate_retrospective_agenda**: Creates a structured meeting or review sequence based on the project's unique composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Project Retrospective Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I've finished my project. Can you help me decide what we should do differently next time?"

**🤖 AI Agent:**
> I will use the `derive_decision_matrix` tool to analyze your project reflections and provide a structured list of what to keep, change, and stop for your future workflows.

---

**👤 You:**
> "Generate a summary of the project for our archives, including the rights status."

**🤖 AI Agent:**
> I am compiling the documentation summary now using `compile_documentation_summary` to ensure all milestones and legal usage details are captured for your records.

---

**👤 You:**
> "Who should we recognize for their contributions to this project?"

**🤖 AI Agent:**
> I will run `execute_acknowledgement_actions` to identify the specific participants who deserve recognition based on the project's successful outcomes and decisions.


## ❓ FAQ

**Q: How can I use this to plan my next project?**
You can use the `formulate_next_direction` tool. It analyzes your current project's unresolved work and your expressed interests to create a strategic brief for your next endeavor.

**Q: What is the purpose of the decision matrix?**
The `derive_decision_matrix` tool synthesizes reflections into a 'Keep, Change, Stop' list, helping you decide which processes to persist and which to abandon based on project data.

**Q: Can I generate a meeting agenda automatically?**
Yes, the `generate_retrospective_agenda` tool creates a structured sequence for your review meetings, prioritizing learning goals and outcome assessments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-project-retrospective-plan](https://vinkius.com/en/ai-agent-connect/creative-project-retrospective-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Project Retrospective Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-project-retrospective-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Project Retrospective Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-project-retrospective-plan": {
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
