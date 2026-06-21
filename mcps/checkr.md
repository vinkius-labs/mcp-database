# Checkr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate background checks via Checkr — screen candidates, monitor reports, and manage compliance directly from any AI agent.

## Description
Connect your **Checkr** account to any AI agent and take full control of your background screening and hiring compliance through natural conversation. Streamline how you screen candidates and verify credentials.

### What you can do

- **Candidate Oversight** — List and retrieve details for all candidates in your account natively
- **Report Intelligence** — Access background check reports and their current status (Clear, Consider, Pending) flawlessly
- **Screening Automation** — Create new candidate profiles and initiate background checks securely
- **Package Logistics** — List and manage available screening packages like 'Pro' and 'Basic' flawlessly
- **Invitation Control** — Monitor invitations sent to candidates to complete their own screening applications securely
- **Compliance Monitoring** — Retrieve detailed report results and adverse action status directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkr API Secret Key (obtained from your dashboard)
3. Start managing your background checks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — monitor background check progress and review candidate statuses using natural language
- **Recruiters** — create new candidates and trigger screenings without opening the dashboard
- **Compliance Officers** — audit report results and verify screening packages straight from their chat interface
- **Operations Teams** — quickly check the status of pending invitations and candidate profiles


## Available Tools
- **create_new_candidate**: Create a new candidate profile
- **start_background_check**: Initiate a background check for a candidate
- **get_candidate_details**: Get detailed information for a specific candidate
- **get_report_details**: Get detailed information for a specific background report
- **list_checkr_candidates**: List candidates in the account
- **list_screening_invitations**: List invitations sent to candidates
- **list_screening_packages**: List available screening packages (e.g. Pro, Basic)
- **list_background_reports**: List background check reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 background checks in my Checkr account."

**🤖 AI Agent:**
> Retrieving recent reports... I found 5 items: John Doe (Clear), Jane Smith (Pending), Mike Miller (Consider), and 2 others. Would you like to see the details for Mike Miller?

---

**👤 You:**
> "Check the status of the candidate named 'Jane Smith'."

**🤖 AI Agent:**
> Searching for Jane Smith... I found 1 profile. Her background check is currently 'Pending' (75% complete). We are waiting for the motor vehicle record check to finish.

---

**👤 You:**
> "What screening packages do I have available?"

**🤖 AI Agent:**
> Checking your available packages... You have 3 configured: 'Standard Pro' (Criminal + MVR), 'Basic' (Criminal Only), and 'Executive' (Standard + Credit + Employment).


## ❓ FAQ

**Q: Can I see if a background check has any issues through the agent?**
Yes! Use the `get_report_details` tool. The agent will return the current status. If the status is 'Consider', it means some records were found that require your review.

**Q: How do I invite a new candidate to start their check?**
First, use `create_new_candidate` to add them to your account, then use `start_background_check` with the appropriate package name to trigger the invitation email.

**Q: Where do I find my Checkr API Secret Key?**
Log in to your Checkr dashboard and navigate to **Settings -> API**. You can generate and copy your Secret Key from the 'API Keys' section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkr](https://vinkius.com/mcp/checkr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Checkr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `checkr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Checkr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "checkr": {
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
