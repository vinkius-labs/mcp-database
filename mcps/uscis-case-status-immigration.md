# USCIS Case Status (Immigration) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uscis-case-status-immigration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track USCIS immigration case statuses and processing history directly from your AI agent using receipt numbers.

## Description
Connect to the official USCIS developer portal to monitor immigration applications. This server allows your AI agent to fetch real-time updates on case statuses, processing history, and current milestones for any valid 13-character receipt number.

### What you can do

- **Real-time Status** — Get the current standing of any USCIS application (e.g., 'Case Was Approved', 'Request for Evidence Sent')
- **Historical Tracking** — Retrieve the full chronological history of actions taken on a specific case
- **Multi-Case Monitoring** — Ask your agent to check multiple receipt numbers in sequence to provide a summary of your entire portfolio
- **Milestone Analysis** — Understand exactly where an application sits in the processing pipeline without logging into the USCIS website

### How it works

1. Subscribe to this server
2. Enter your USCIS Developer Client ID, Secret, and Environment
3. Provide a 13-character receipt number (e.g., EAC, LIN, MSC, SRC, WAC, IOE)

### Who is this for?

- **Immigration Attorneys** — quickly check status updates for multiple clients directly from a chat interface or document editor
- **Applicants** — stay informed about your personal Green Card, Visa, or Citizenship application progress via natural language
- **HR & Global Mobility Teams** — monitor employee sponsorship cases and filing histories efficiently


## Available Tools
- **get_case_status**: Get USCIS case status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USCIS Case Status (Immigration)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of USCIS case EAC9999103402."

**🤖 AI Agent:**
> I've retrieved the status for EAC9999103402. It is currently 'Case Was Approved' as of October 12, 2023.

---

**👤 You:**
> "What is the history for case number LIN2190345678?"

**🤖 AI Agent:**
> The history for LIN2190345678 shows 3 major events: 1. Case Received (Jan 5), 2. Biometrics Appointment (Feb 10), and 3. Case is Being Actively Reviewed (Feb 12).

---

**👤 You:**
> "Give me the latest update on my immigration application MSC2290123456."

**🤖 AI Agent:**
> The latest update for MSC2290123456 is 'Request for Additional Evidence Was Sent' on March 15, 2024. You should expect a notice in the mail.


## ❓ FAQ

**Q: How do I track a specific immigration application?**
Use the `get_case_status` tool with your 13-character receipt number (e.g., EAC1234567890). Your agent will return the current status and the date of the last update.

**Q: Does this server provide the history of the case?**
Yes, the `get_case_status` tool returns both the current status and the chronological history of actions taken on the case by USCIS.

**Q: What happens if I enter an invalid receipt number?**
The `get_case_status` tool will return an error or a message indicating the case was not found. Ensure you are using the correct 13-character format starting with letters like EAC, LIN, or IOE.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uscis-case-status-immigration](https://vinkius.com/mcp/uscis-case-status-immigration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USCIS Case Status (Immigration)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `uscis-case-status-immigration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USCIS Case Status (Immigration)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uscis-case-status-immigration": {
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
