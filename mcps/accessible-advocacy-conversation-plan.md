# Accessible Advocacy Conversation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-advocacy-conversation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured, facts-first advocacy strategies for accessibility needs.

## Description
This MCP server provides a suite of tools to help users navigate accessibility barriers using facts-first communication and minimum necessary disclosure. It enables users to `generate_conversation_agenda` for professional meetings, `draft_request_wording` for clear verbal or written scripts, `create_evidence_checklist` to prepare verifiable proof, `record_agreed_next_steps` to ensure accountability, and `plan_followup_sequence` to track progress on requested changes.


## Available Tools (5)
- **create_evidence_checklist**: Helps prepare tangible proof to support claims
- **draft_request_wording**: Generates specific language for articulating needs
- **generate_conversation_agenda**: Provides a structured roadmap for the meeting or interaction
- **plan_followup_sequence**: Provides a schedule for checking in on progress
- **record_agreed_next_steps**: Creates a formal record of what was decided


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Advocacy Conversation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to talk to my manager about a broken elevator in the office. I have a formal relationship with them."

**🤖 AI Agent:**
> I have generated a structured agenda for your meeting. It includes an opening to present the factual observation of the elevator malfunction, followed by the specific request for repair, and a closing to confirm the timeline for the fix.

---

**👤 You:**
> "Help me write an email to a service provider about a website that isn't screen-reader friendly. I want to keep it direct and use minimum disclosure."

**🤖 AI Agent:**
> Here is your written email draft: 'I am writing to report an accessibility barrier on your website. The current navigation structure is not compatible with screen readers, preventing full access to the service. I request that the navigation elements be updated to meet accessibility standards.'

---

**👤 You:**
> "My boss agreed to provide a quiet workspace by next Friday. How should I follow up?"

**🤖 AI Agent:**
> I have created a follow-up sequence. Since your relationship is professional, I recommend a brief check-in on Wednesday to confirm the workspace is ready for your use on Friday.


## ❓ FAQ

**Q: How does this tool help with accessibility requests?**
It provides structured tools like `generate_conversation_agenda` and `draft_request_wording` to help you communicate needs clearly and professionally using objective facts.

**Q: What is 'Minimum Necessary Disclosure'?**
It is a principle used in `draft_request_wording` to ensure you only share the specific information required to address the barrier, protecting your privacy.

**Q: Can I use this to track what was promised in a meeting?**
Yes, you can use `record_agreed_next_steps` to create a formal record of decisions and `plan_followup_sequence` to schedule check-ins.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-advocacy-conversation-plan](https://vinkius.com/en/ai-agent-connect/accessible-advocacy-conversation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Advocacy Conversation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-advocacy-conversation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Advocacy Conversation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-advocacy-conversation-plan": {
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
