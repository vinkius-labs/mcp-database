# Care Decision Meeting Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-decision-meeting-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Structures clinical decision-making meetings with agendas, pre-reads, and decision logs.

## Description
This MCP server provides specialized coordination tools for healthcare professionals to manage complex clinical decision-making. It enables the generation of structured meeting agendas using `generate_meeting_agenda`, identifies essential evidence via `compile_pre_read_list`, formalizes outcomes with `record_decision`, and tracks subsequent tasks through `assign_follow_up_actions`. It ensures multidisciplinary alignment and patient safety by applying specific governance rules like Consensus, Consent, or Majority.


## Available Tools (4)
- **compile_pre_read_list**: Identifies what documents and data must be reviewed before the meeting starts
- **generate_meeting_agenda**: Creates a structured chronological timeline for the meeting
- **record_decision**: Formalizes a decision made during the meeting into a permanent log
- **assign_follow_up_actions**: Generates a list of tasks and subsequent review dates resulting from the decisions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Decision Meeting Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 30-minute agenda for a meeting with Dr. Smith and Nurse Jones to discuss discharge plans, prioritizing the discharge plan."

**🤖 AI Agent:**
> Meeting Agenda:
- Discharge Plan Discussion: 25 minutes
- Other items: 5 minutes
Total Duration: 30 minutes

---

**👤 You:**
> "What documents should we review for a decision on palliative care transition?"

**🤖 AI Agent:**
> Required Documents: Patient History, Recent Lab Results, Imaging Reports.

---

**👤 You:**
> "Record the decision to transition to palliative care using Consensus with Dr. Smith and Nurse Jones."

**🤖 AI Agent:**
> Decision Recorded: Transition to palliative care. Outcome: Approved. Rationale: Patient comfort and goals of care alignment. Rule: Consensus. Participants: Dr. Smith, Nurse Jones.


## ❓ FAQ

**Q: How does this tool help with clinical governance?**
The `record_decision` tool allows users to specify the governance rule used, such as Consensus or Consent, ensuring every clinical decision is documented with its specific rationale and rule.

**Q: Can I prepare participants before the meeting starts?**
Yes, you can use `compile_pre_read_list` to identify which supporting documents are essential for the decisions being discussed, helping participants prepare in advance.

**Q: How are follow-up tasks managed?**
After decisions are finalized, `assign_follow_up_actions` generates a list of tasks and maps them to specific review dates to ensure implementation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-decision-meeting-plan](https://vinkius.com/en/ai-agent-connect/care-decision-meeting-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Decision Meeting Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-decision-meeting-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Decision Meeting Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-decision-meeting-plan": {
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
