# Local History Project Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-history-project-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [research](../categories/research.md)

A management engine for organizing community history research, ensuring ethical compliance and structured milestones.

## Description
This MCP server provides a complete toolkit for managing community history research projects. It handles the entire lifecycle from initial planning to final presentation. Use `generate_research_plan` to build a roadmap, `compose_outreach_message` to contact participants, and `validate_consent_status` to ensure all research activities meet ethical standards. The server also includes tools to record findings via `create_evidence_log_entry` and organize public dissemination with `schedule_presentation`.


## Available Tools (5)
- **create_evidence_log_entry**: Records a new piece of historical evidence or a participant interaction
- **generate_research_plan**: Creates a comprehensive roadmap for the project based on initial user inputs
- **schedule_presentation**: Organizes the final dissemination of research findings
- **validate_consent_status**: Checks if a specific contributor or location has provided the necessary permissions
- **compose_outreach_message**: Generates professional communication for potential participants or site managers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local History Project Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 4-week research plan for the history of the Old Mill, focusing on the river site and involving local historians."

**🤖 AI Agent:**
> I have generated a 4-week research plan for the Old Mill project. The plan includes discovery phases at the river site and scheduled interviews with the local historians.

---

**👤 You:**
> "Write an email to Sarah Jenkins to ask for an interview about the town's founding."

**🤖 AI Agent:**
> Subject: Invitation to participate in local history research

Dear Sarah Jenkins,

I am reaching out to request an interview regarding the history of the town's founding. Your insights would be invaluable to our research project.

---

**👤 You:**
> "Check if the Old Library has given permission for photography."

**🤖 AI Agent:**
> The Old Library has provided explicit permission for photography. The consent is valid and cleared for use in your research.


## ❓ FAQ

**Q: How do I start a new research project?**
You can start by using the `generate_research_plan` tool, which creates a structured roadmap based on your topic, locations, and timeline.

**Q: How does the server handle participant consent?**
The server enforces strict ethical compliance. You must use `validate_consent_status` to verify that a contributor has provided explicit permission before recording any evidence.

**Q: Can I use this to organize public presentations?**
Yes, the `schedule_presentation` tool allows you to organize the final dissemination of your findings to audiences like community boards or libraries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-history-project-manager](https://vinkius.com/en/ai-agent-connect/local-history-project-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local History Project Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-history-project-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local History Project Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-history-project-manager": {
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
