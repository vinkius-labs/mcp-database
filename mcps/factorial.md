# Factorial MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/factorial)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage HR operations via Factorial — list employees and teams, track leave requests, monitor shifts and payslips, and handle company documents directly from any AI agent.

## Description
Connect your **Factorial HR** account to any AI agent and take full control of your human resources management and organizational workflows through natural conversation.

### What you can do

- **Employee & Team Orchestration** — List all registered employees and teams to retrieve detailed profiles, organizational roles, and department structures natively
- **Leave & Absence Monitoring** — Fetch all holiday and leave requests for any given year to track team availability and upcoming time-off boundaries flawlessly
- **Shift & Schedule Navigation** — Retrieve detailed shift scheduling information for specific months to audit team rotations and operational coverage securely
- **Payroll Oversight** — List available payslips across the organization for specific months to verify compensation records and financial trail metadata
- **Document Discovery** — Access stored company documents and folders to retrieve HR policies and internal documentation using natural language
- **Company Data Auditing** — Fetch global company metadata and administrative configurations to verify workspace settings and organizational identities
- **Personnel Intelligence** — Resolve specific employee contexts including contact details, manager relationships, and hiring dates limitlessly

### How it works

1. Subscribe to this server
2. Enter your Factorial API Key (found in Settings > Advanced configuration > API Keys)
3. Start managing your HR operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — track leave requests and monitor employee directories without opening the Factorial dashboard
- **Team Leads** — check team availability and audit shift schedules using natural language conversation
- **Finance Teams** — verify payslip availability and audit company metadata in real-time
- **Operations Teams** — manage company documents and verify organizational structures through the chat interface


## Available Tools (12)
- **clock_in**: Clock in for a shift
- **clock_out**: Clock out from a shift
- **get_employee**: Get a specific Factorial employee by ID
- **get_me**: Get current company identity info
- **list_documents**: List all company documents
- **list_employees**: List all Factorial employees
- **list_folders**: List all company folders
- **list_holidays**: List all holidays for a given year
- **list_leaves**: List all leaves for a given year
- **list_payslips**: List all payslips for a given year and month
- **list_shifts**: List all shifts for a given year and month
- **list_teams**: List all Factorial teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Factorial** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the 'Engineering' team"

**🤖 AI Agent:**
> Retrieving 'Engineering' members... I found 15 employees including 'John Smith' (Lead), 'Jane Doe' (Senior Dev), and 'Alice Wong'. Would you like the contact details or manager info for any of them?

---

**👤 You:**
> "Show me upcoming leave requests for June 2026"

**🤖 AI Agent:**
> Checking June 2026... There are 3 approved leave requests: 'Jane Doe' (June 1-5), 'Robert Brown' (June 15-20), and 'Sarah Connor' (June 22-26). Your team availability is currently at 80% for that month.

---

**👤 You:**
> "Find HR policy documents in the company folders"

**🤖 AI Agent:**
> Searching company documents... I found 2 related files: '2024_Remote_Work_Policy.pdf' and 'Global_Benefits_Guide.pdf'. Would you like the download link or a summary of the remote work policy?


## ❓ FAQ

**Q: Can my agent list all leave requests for the current year in Factorial?**
Yes. Use the 'list_leaves' tool. You can specify the 'year' parameter, and the agent will fetch all absence and holiday requests, allowing you to track team availability flawlessly.

**Q: How do I check the shift schedule for a specific month via chat?**
Use the 'list_shifts' tool. Provide the 'year' and 'month' (numeric). The agent will retrieve the detailed scheduling information, providing you with a clear view of operational coverage.

**Q: Can I audit payslip availability through the agent?**
Absolutely. Use the 'list_payslips' tool for a target year and month. Your agent will verify which employees have available compensation records without you needing to manually navigate the payroll section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/factorial](https://vinkius.com/mcp/factorial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Factorial** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `factorial` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Factorial** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "factorial": {
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
