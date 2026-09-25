# Interview-Based Story Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/interview-based-story-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic planning engine for journalistic and qualitative storytelling workflows.

## Description
This MCP server provides a structured framework for managing the lifecycle of an interview-based story. It enforces strict consent and attribution boundaries to ensure ethical compliance. Users can `generate_outreach_sequence` to plan communications, `create_session_agenda` to prepare for interviews, `log_permission_record` to track formal consent, `develop_narrative_steps` to organize story development, and `define_review_options` to manage participant feedback.


## Available Tools (5)
- **create_session_agenda**: Generates a structured guide for conducting the interview
- **define_review_options**: Determines how participants can review the final output
- **develop_narrative_steps**: Provides a step-by-step workflow to move from interview to finished story
- **generate_outreach_sequence**: Creates a timeline of communications to secure interviewees
- **log_permission_record**: Creates an immutable-style record of what a participant has allowed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Interview-Based Story Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to interview three experts about climate change over the next two weeks. Can you help me plan the outreach?"

**🤖 AI Agent:**
> I have generated an outreach sequence for your three experts, scheduled to complete within your two-week window, including initial contact and follow-up steps.

---

**👤 You:**
> "Help me prepare for an interview about urban planning. The topics are zoning, public transit, and green spaces. The source has requested full attribution."

**🤖 AI Agent:**
> I have created a session agenda covering zoning, public transit, and green spaces, with a prioritized section at the beginning to confirm consent and recording preferences.

---

**👤 You:**
> "I need to log that Jane Doe has given permission for her full name to be used, but only for internal reports."

**🤖 AI Agent:**
> The permission record for Jane Doe has been logged, specifying full attribution with usage limited to internal reports.


## ❓ FAQ

**Q: How does this tool handle participant consent?**
The tool uses `log_permission_record` to create an immutable record of all permissions, ensuring that all subsequent narrative steps respect the established consent and attribution rules.

**Q: Can I use this to plan my interview schedule?**
Yes, you can use `generate_outreach_sequence` to create a chronological timeline of communications to secure your interviewees based on your specific project timeline.

**Q: What happens if I need to change the story structure?**
You can use `develop_narrative_steps` to generate a new workflow that aligns with your updated story purpose and attribution requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/interview-based-story-plan](https://vinkius.com/en/ai-agent-connect/interview-based-story-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Interview-Based Story Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `interview-based-story-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Interview-Based Story Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "interview-based-story-plan": {
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
