# Global Scholarship Deadline Tracker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/global-scholarship-deadline-tracker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/global-scholarship-deadline-tracker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/global-scholarship-deadline-tracker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Instantly calculate urgency and generate comprehensive document checklists for global scholarships (FUVEST, Erasmus+, DAAD).

## Description
**Problem:** Tracking deadlines across multiple international scholarship programs (like Fulbright, Erasmus+, and DAAD) is complex. Each program has unique rules, varying document requirements, and non-standardized timelines. Missing a single deadline can mean losing the opportunity.


## Available Tools
- **calculate_deadline_calendar**: Returns events sorted by earliest deadline first, with days remaining calculated from today.

Calculate deadline urgency and generate sorted calendar
- **generate_document_checklist**: Mandatory global documents appear first in the list.

Generate document checklist for a scholarship and region
- **get_scholarship_opportunity**: Use this to look up deadlines for FUVEST, PROUNI, SISU, Fulbright, ErasmusPlus, or DAAD programs.

Retrieve scholarship opportunity details by ID and year


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


## Installation & Usage

To install and use the **Global Scholarship Deadline Tracker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/global-scholarship-deadline-tracker](https://vinkius.com/mcp/global-scholarship-deadline-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
