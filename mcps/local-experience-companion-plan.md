# Local Experience Companion Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-companion-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social](../categories/social.md)

Coordinate local activities with companions through mutual agreement and role-based planning.

## Description
This MCP server acts as a coordination engine to synchronize user activities with companion candidates. It applies mutual consent, role definitions, and logistical requirements to generate comprehensive engagement plans. Users can use `plan_companion_arrangement` to find suitable matches, `generate_role_briefing` to define specific duties and boundaries, `execute_handoff` to prepare for meetings, and `process_cancellation` to manage terminations respectfully.


## Available Tools (4)
- **execute_handoff**: Generate the immediate instructions and summary for the moment the user and companion meet
- **generate_role_briefing**: Provide a detailed instruction set for the companion so they understand their specific responsibilities and limits
- **plan_companion_arrangement**: Find a suitable companion and create a complete engagement plan based on user requirements and candidate availability
- **process_cancellation**: Manage the termination of a planned activity while maintaining respect and adhering to cost agreements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Companion Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to a museum tomorrow afternoon. Can you find a companion who can help with navigation?"

**🤖 AI Agent:**
> I have found a suitable companion for your museum visit tomorrow afternoon. The arrangement includes navigation support as requested.

---

**👤 You:**
> "I need to cancel my planned coffee meeting because I am feeling unwell."

**🤖 AI Agent:**
> The cancellation has been processed. A respectful message has been sent to your companion, and any applicable fees have been calculated.

---

**👤 You:**
> "I am ready to meet my companion at the central park entrance."

**🤖 AI Agent:**
> Here are your handoff details: you will meet at the central park entrance, and your companion is prepared to fulfill the agreed roles.


## ❓ FAQ

**Q: How do I find a companion for my activity?**
You can use the `plan_companion_arrangement` tool to match your activity, availability, and cost preferences with available companion candidates.

**Q: Can I set specific boundaries for the companion?**
Yes, you can define explicit consent boundaries during the planning phase to ensure the companion respects your personal space and needs.

**Q: What happens if I need to cancel an arrangement?**
You can use `process_cancellation` to manage the termination. The system will handle any necessary fees based on the timing and the agreed-upon cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-companion-plan](https://vinkius.com/en/ai-agent-connect/local-experience-companion-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Companion Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-companion-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Companion Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-companion-plan": {
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
