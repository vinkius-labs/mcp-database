# HackerOne MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hackerone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate bug bounty management via HackerOne — manage reports, programs, and payments directly from any AI agent.

## Description
Connect your **HackerOne** organization account to any AI agent and take full control of your vulnerability management workflows through natural conversation.

### What you can do

- **Report Oversight** — List all vulnerability reports, retrieve detailed information, and monitor their current state and severity.
- **Program Insights** — Browse your bug bounty or VDP programs and access structured scopes and assets.
- **Report Interaction** — Add comments to reports, change their triaged state, or award bounties directly from the chat.
- **Asset Tracking** — Monitor the assets defined within your security programs and their reachability.
- **Financial Monitoring** — Retrieve history of bounty payments and manage rewards efficiently.
- **Hacktivity Feed** — Stay updated with the internal or public hacktivity feed to see recent discoveries.

### How it works

1. Subscribe to this server
2. Enter your HackerOne API Token Identifier and Token Value
3. Start managing your security programs from Claude, Cursor, or any MCP-compatible client

No more jumping between report tabs. Your AI assistant acts as a dedicated Triage Engineer or Security Program Manager.

### Who is this for?

- **Security Engineers** — instantly retrieve report details and severity ratings during triage.
- **Bug Bounty Managers** — automate the process of awarding bounties and communicating with researchers.
- **CISOs** — maintain a real-time overview of incoming vulnerabilities and program health.


## Available Tools (10)
- **add_report_comment**: Add a comment to a specific vulnerability report
- **award_bounty**: Award a bounty for a vulnerability report
- **change_report_state**: Update the state of a vulnerability report (e.g., triaged, resolved)
- **get_program**: Get details for a specific security program
- **get_report**: Get detailed information about a specific vulnerability report
- **list_assets**: List assets defined in your security programs
- **list_hacktivity**: List the HackerOne hacktivity feed
- **list_payments**: List bounty payments history
- **list_programs**: List bug bounty or VDP programs you have access to
- **list_reports**: List vulnerability reports submitted to your HackerOne program


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HackerOne** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vulnerability reports submitted this week."

**🤖 AI Agent:**
> I've retrieved your reports. You have 5 new submissions this week, including 'SQL Injection in /api/v1/users' (High) and 'BOLA in account settings' (Medium). Would you like to see the details for the High severity report?

---

**👤 You:**
> "Award a $500 bounty to report ID 12345."

**🤖 AI Agent:**
> Bounty awarded! I've successfully processed a $500 reward for report 12345. The researcher has been notified. Should I add a comment to the report as well?

---

**👤 You:**
> "Change the state of report 12345 to 'Triaged'."

**🤖 AI Agent:**
> State updated! Report 12345 is now marked as 'Triaged'. I've also added an internal note for the security team. What's the next step for this report?


## ❓ FAQ

**Q: How do I generate my HackerOne API Token?**
Log in to HackerOne, navigate to **Settings > API Token**, and click 'Create API Token'. Make sure to copy both the **Identifier** and the **Token Value** immediately.

**Q: Can I award bounties through this integration?**
Yes! Use the `award_bounty` tool by providing the report ID and the amount. You can also specify an optional bonus amount for the researcher.

**Q: Does the integration support internal comments?**
Yes, the `add_report_comment` tool has an optional `internal` boolean parameter (defaults to true). This allows you to communicate with your team privately on a specific report.

**Q: Can I filter reports by their handle or ID?**
You can use `list_reports` to see all reports or `get_report` with a specific ID to retrieve detailed information for a single discovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hackerone](https://vinkius.com/mcp/hackerone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HackerOne** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hackerone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HackerOne** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hackerone": {
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
