# Family Care Update Digest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-care-update-digest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Consolidate caregiver updates into structured, privacy-compliant weekly digests and actionable schedules.

## Description
This MCP server connects AI agents to caregiver workflows. It processes raw, unstructured notes into organized summaries, expense reports, and upcoming schedules. Using `analyze_care_updates`, agents can extract tasks and appointments from messy text. The `apply_privacy_filter` tool ensures sensitive medical or financial data is redacted based on the recipient's role. Finally, `generate_weekly_digest` produces a clean, shareable report, while `extract_next_week_schedule` provides a focused view of upcoming needs.


## Available Tools (4)
- **apply_privacy_filter**: Redacts or generalizes information based on the chosen privacy level
- **analyze_care_updates**: Processes raw caregiver notes into a structured internal state
- **extract_next_week_schedule**: Isolates upcoming appointments and tasks to create a focused forward-looking view
- **generate_weekly_digest**: Produces the final, human-readable, shareable text document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Care Update Digest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these notes: 'Mom had a doctor visit today. Spent $50 on meds. Need to schedule physical therapy for next Tuesday.'"

**🤖 AI Agent:**
> Summary: Mom had a doctor visit. Completed: Doctor visit. Pending: Schedule physical therapy. Expenses: $50 for medication. Next Week: Physical therapy on Tuesday.

---

**👤 You:**
> "Extract the schedule for next week from these updates starting 2024-06-01."

**🤖 AI Agent:**
> Upcoming events for next week: Physical therapy on June 4th.

---

**👤 You:**
> "Filter this data for a family member: 'Patient has hypertension. Paid $120 for specialist.'"

**🤖 AI Agent:**
> Summary: Health update provided. Expenses: Medical costs incurred.


## ❓ FAQ

**Q: How does this tool handle sensitive medical information?**
You can use `apply_privacy_filter` to redact or generalize sensitive details. By selecting different audience types, you can ensure that medical or financial data is only visible to authorized primary caregivers.

**Q: Can I generate a schedule for the upcoming week?**
Yes, the `extract_next_week_schedule` tool isolates upcoming appointments and high-priority tasks to create a focused forward-looking view.

**Q: What format will the final digest be in?**
The `generate_weekly_digest` tool produces a human-readable text document organized by Summary, Completed, Pending, Expenses, and Schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-care-update-digest](https://vinkius.com/en/ai-agent-connect/family-care-update-digest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Care Update Digest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-care-update-digest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Care Update Digest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-care-update-digest": {
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
