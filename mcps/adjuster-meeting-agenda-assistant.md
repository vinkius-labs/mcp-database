# Adjuster Meeting Agenda Assistant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/adjuster-meeting-agenda-assistant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize insurance claim meetings by prioritizing topics based on loss complexity and policy constraints.

## Description
This MCP server helps insurance adjusters prepare for meetings by transforming loss details, unresolved questions, and policy excerpts into a structured, time-constrained agenda. It uses `generate_agenda` to prioritize topics by urgency--focusing on coverage disputes and critical evidence--and `validate_agenda_feasibility` to ensure the meeting stays within the allocated time. Adjusters can also use `analyze_coverage_priority` to identify high-risk questions and `map_evidence_to_topics` to link specific documents to relevant discussion points.


## Available Tools (4)
- **generate_agenda**: Create a structured meeting agenda prioritized by importance and constrained by time
- **analyze_coverage_priority**: Identify which unresolved questions or loss details pose the highest risk to the claim timeline
- **map_evidence_to_topics**: Link specific documents to the most relevant agenda topics
- **validate_agenda_feasibility**: Check if the proposed agenda is realistic given the time constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adjuster Meeting Agenda Assistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an agenda for a 30-minute meeting regarding a water damage claim. We have a repair estimate and a photo of the damage. We need to discuss if the pipe burst is covered under the current policy."

**🤖 AI Agent:**
> 1. Coverage Discussion: Pipe burst liability (15 mins) - Evidence: Photo of damage. Outcome: Determine if the incident falls under covered perils.
2. Damage Assessment (10 mins) - Evidence: Repair estimate. Outcome: Review estimated costs.
3. Next Steps (5 mins). Total: 30 mins.

---

**👤 You:**
> "Which of these questions is most critical for a 45-minute meeting about a theft claim? Questions: 1. When was the police report filed? 2. Does the policy cover jewelry theft? 3. What is the claimant's phone number?"

**🤖 AI Agent:**
> The most critical question is: 'Does the policy cover jewelry theft?', as it directly impacts coverage determination.

---

**👤 You:**
> "Check if this agenda is feasible for a 20-minute meeting: Topic A (10 mins), Topic B (15 mins)."

**🤖 AI Agent:**
> No, the agenda is not feasible. The total required time is 25 minutes, which exceeds the 20-minute limit (including the required buffer).


## ❓ FAQ

**Q: How does the tool prioritize meeting topics?**
The tool prioritizes topics based on urgency: coverage disputes and missing critical evidence are ranked highest, followed by unresolved questions and itemization.

**Q: Can I ensure my meeting won't run over time?**
Yes, the `validate_agenda_feasibility` tool checks the proposed agenda against your meeting duration, including a built-in buffer.

**Q: How do I link my documents to the agenda?**
You can use the `map_evidence_to_topics` tool to automatically link your available evidence list to the specific topics identified in your agenda.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/adjuster-meeting-agenda-assistant](https://vinkius.com/en/ai-agent-connect/adjuster-meeting-agenda-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adjuster Meeting Agenda Assistant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adjuster-meeting-agenda-assistant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adjuster Meeting Agenda Assistant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adjuster-meeting-agenda-assistant": {
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
