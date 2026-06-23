# MaestroQA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maestroqa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Access quality assurance reviews, QA scores, and export performance data via the MaestroQA API.

## Description
Connect your **MaestroQA** account to any AI agent to automate your customer service quality assurance and performance reporting. This MCP server enables your agent to list tickets, monitor QA scores, request detailed data exports, and sync external CSAT scores directly from natural language interfaces.

### What you can do

- **Score Monitoring** — List support tickets and retrieve real-time Internal Quality Scores (IQS) and grading statuses
- **Automated Exporting** — Initialize asynchronous raw data exports for deep analysis of rubric answers and performance
- **Agent Oversight** — List all support agents and available evaluation rubrics to organize your QA process
- **CSAT Synchronization** — Push external customer satisfaction scores into MaestroQA to correlate them with internal QA grades
- **Detailed Auditing** — Retrieve complete metadata and scoring breakdowns for any individual ticket

### How it works

1. Subscribe to this server
2. Enter your MaestroQA (Rippit) API Token
3. Start managing your support quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — Monitor support quality trends and export grading data via simple natural language commands
- **Support Leads** — Quickly audit agent performance and identify tickets awaiting review from your dev tools
- **Operations Teams** — Automate the synchronization of CSAT data and maintain accurate quality reporting effortlessly


## Available Tools (7)
- **list_qa_agents**: List all agents tracked in MaestroQA
- **get_export_download_links**: Retrieve links for a requested export
- **get_ticket_qa_details**: Get QA details for a specific ticket
- **push_csat_scores**: Sync external CSAT scores into MaestroQA
- **request_qa_data_export**: Requires start_date and end_date.

Initialize a raw QA data export (Async)
- **list_qa_rubrics**: List all available evaluation rubrics
- **list_qa_tickets**: Use optional params for filtering.

List tickets and their QA statuses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MaestroQA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all support tickets awaiting QA review in MaestroQA."

**🤖 AI Agent:**
> I've retrieved the list of tickets. You have 15 tickets currently marked as 'Pending', including Ticket #12345 from 'Support Team A'. Would you like to see the full metadata for any of them?

---

**👤 You:**
> "Request a raw data export for the month of July in MaestroQA."

**🤖 AI Agent:**
> I've submitted the export request for July (Start: 2024-07-01, End: 2024-07-31). The export ID is 'exp-98765'. I will check for the download links shortly.

---

**👤 You:**
> "Show the QA score for ticket ID 'ticket-54321'."

**🤖 AI Agent:**
> I've retrieved the details for ticket 54321. The Internal Quality Score (IQS) is 🟢 95%. It was graded on 2024-08-15 using the 'Global Support Rubric'.


## ❓ FAQ

**Q: What is an Internal Quality Score (IQS)?**
IQS is the grade assigned to a ticket during the QA process based on your rubrics. The agent can retrieve this score using the `get_ticket_qa_details` tool.

**Q: How do I download a data export?**
First, request the export using `request_qa_data_export`. Once processed, use `get_export_download_links` with the provided ID to retrieve the download URL.

**Q: Where do I find my API Token?**
Log in to MaestroQA, go to Settings > API, and generate a new token. Note that the API is also referred to as 'Rippit' in technical documentation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maestroqa](https://vinkius.com/mcp/maestroqa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MaestroQA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maestroqa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MaestroQA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maestroqa": {
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
