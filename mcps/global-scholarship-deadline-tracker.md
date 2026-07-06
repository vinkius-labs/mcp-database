# Global Scholarship Deadline Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/global-scholarship-deadline-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Instantly calculate urgency and generate comprehensive document checklists for global scholarships (FUVEST, Erasmus+, DAAD).

## Description
**Problem:** Tracking deadlines across multiple international scholarship programs (like Fulbright, Erasmus+, and DAAD) is complex. Each program has unique rules, varying document requirements, and non-standardized timelines. Missing a single deadline can mean losing the opportunity.


## Available Tools (3)
- **get_scholarship_opportunity**: Use this to look up deadlines for FUVEST, PROUNI, SISU, Fulbright, ErasmusPlus, or DAAD programs.

Retrieve scholarship opportunity details by ID and year
- **calculate_deadline_calendar**: Returns events sorted by earliest deadline first, with days remaining calculated from today.

Calculate deadline urgency and generate sorted calendar
- **generate_document_checklist**: Mandatory global documents appear first in the list.

Generate document checklist for a scholarship and region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Global Scholarship Deadline Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am interested in Fulbright for 2025. What are the core dates?"

**🤖 AI Agent:**
> Running `get_scholarship_opportunity(scholarshipId='Fulbright', targetYear=2025)` shows that the closing date is [Date]. You should prioritize this.

---

**👤 You:**
> "Check my deadlines for FUVEST, Erasmus+, and PROUNI using the 2025 data."

**🤖 AI Agent:**
> Passing the list to `calculate_deadline_calendar` shows that FUVEST has the most urgent deadline, with only [X] days remaining. The calendar is sorted by urgency.

---

**👤 You:**
> "I need a document list for DAAD in Europe for my application."

**🤖 AI Agent:**
> The required documents for DAAD in EUROPE are: Passport copy (GLOBAL), Academic Transcripts, and Statement of Purpose. Use `generate_document_checklist(scholarshipId='DAAD', targetRegion='EUROPE')` to confirm this list.


## ❓ FAQ

**Q: How do I find the basic details and dates for a specific scholarship?**
Use the `get_scholarship_opportunity` tool. You must provide the unique `scholarshipId` (e.g., 'Fulbright') and the `targetYear`. This function retrieves core metadata, including both start and end dates for your program.

**Q: I have a list of scholarships. How do I know which one is the most urgent?**
Pass your list of scholarship names and end dates to the `calculate_deadline_calendar` tool. It processes all entries, calculates the days remaining from today, and returns a master calendar sorted by the earliest deadline first. This immediately highlights what needs attention.

**Q: What documents do I need for a specific program, like DAAD in Europe?**
Use the `generate_document_checklist` tool. You must provide the `scholarshipId` and specify the correct `targetRegion` (e.g., 'EUROPE'). This function generates a comprehensive checklist, ensuring mandatory global documents appear at the top.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/global-scholarship-deadline-tracker](https://vinkius.com/mcp/global-scholarship-deadline-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Global Scholarship Deadline Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `global-scholarship-deadline-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Global Scholarship Deadline Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "global-scholarship-deadline-tracker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
