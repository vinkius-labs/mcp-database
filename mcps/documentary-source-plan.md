# Documentary Source Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/documentary-source-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media](../categories/media.md)

A production management system for mapping source usage, outreach, and verification.

## Description
This MCP server provides a comprehensive production management system for documentary filmmakers. It transforms raw inputs into actionable workflows for source utilization, ethical communication, and factual verification. Use `get_source_use_plan` to map how materials fit your narrative, `generate_outreach_actions` to manage interviewee logistics, and `get_verification_questions` to cross-reference claims against source materials. It also includes tools for maintaining an `get_editorial_decision_log` and a `get_participant_communication_plan` to ensure all production decisions align with your editorial boundary.


## Available Tools (5)
- **get_editorial_decision_log**: Document and review the rationale behind narrative and creative choices
- **get_participant_communication_plan**: Organize how and when to communicate with subjects and interviewees
- **generate_outreach_actions**: Create a checklist of logistical steps for engaging with potential interviewees
- **get_source_use_plan**: Determine how specific materials can be legally and narratively integrated into the film
- **get_verification_questions**: Generate a list of investigative questions to validate claims made by sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Documentary Source Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have footage of a protest but only have Tier 2 permission. How should I use it?"

**🤖 AI Agent:**
> Based on your Tier 2 permission, the footage should be used only within the specific geographic regions and time durations defined in your source-consent documentation.

---

**👤 You:**
> "Help me plan my outreach for three primary subjects."

**🤖 AI Agent:**
> Your outreach priority is set to High for the three primary subjects. You should begin with initial inquiries, followed by technical checks and formal scheduling.

---

**👤 You:**
> "Is the claim that the event happened in 1992 verified?"

**🤖 AI Agent:**
> The current credibility score is low; you need to cross-reference this claim with official archival documents or secondary witness accounts to satisfy verification.


## ❓ FAQ

**Q: How does this help with ethical production?**
The server includes tools like `get_participant_communication_plan` to manage consent and `get_source_use_plan` to ensure materials are used within their granted permissions.

**Q: Can I use this to verify facts?**
Yes, the `get_verification_questions` tool generates investigative questions to validate claims against your available source materials.

**Q: How do I track my creative choices?**
You can use `get_editorial_decision_log` to record the rationale behind narrative decisions and ensure they stay within your defined editorial boundary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/documentary-source-plan](https://vinkius.com/en/ai-agent-connect/documentary-source-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Documentary Source Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `documentary-source-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Documentary Source Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "documentary-source-plan": {
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
