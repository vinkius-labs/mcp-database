# Bugcrowd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugcrowd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage crowdsourced security via Bugcrowd — track submissions, programs, and targets directly from any AI agent.

## Description
Connect your **Bugcrowd** account to any AI agent and orchestrate your vulnerability management, bug bounty programs, and security engagements through natural conversation.

### What you can do

- **Submission Oversight** — List and retrieve detailed metadata for all vulnerability reports (submissions) across your programs.
- **Program Management** — List all active security programs and retrieve detailed metadata, including scopes and rewards.
- **Engagement Tracking** — Monitor crowd executions like specific Bug Bounties or Pen Tests directly from your workspace.
- **Target Coordination** — List and inspect assets in scope (targets) for your organization or specific programs.
- **Submission Creation** — Create new vulnerability submissions from external sources using natural language.
- **Organizational Insights** — Retrieve core organization information and settings straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Bugcrowd API Access Token
3. Start managing your crowdsourced security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers & Analysts** — quickly check submission statuses or program scopes without manual dashboard work.
- **Vulnerability Managers** — retrieve and triage reports straight from their workflow tools.
- **CisOs & Security Leads** — monitor program health and target coverage using natural language.


## Available Tools
- **create_submission**: Create a new vulnerability submission
- **get_engagement**: Get details of a specific engagement
- **get_organization_info**: Retrieve core organization information
- **get_program**: Get details of a specific security program
- **get_submission**: Get details of a specific submission
- **get_target**: Get details of a specific target
- **list_engagements**: List all crowd engagements (bounties, pen tests)
- **list_programs**: List all security programs
- **list_submissions**: List all vulnerability submissions
- **list_targets**: List all assets in scope (targets)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bugcrowd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active security programs in Bugcrowd."

**🤖 AI Agent:**
> I've retrieved your programs. You have 3 active programs: 'Vinkius Bounty' (ID: prog_1), 'Main Web App' (ID: prog_2), and 'Legacy Systems' (ID: prog_3).

---

**👤 You:**
> "Show the last 5 vulnerability submissions."

**🤖 AI Agent:**
> Retrieving submissions... Your 5 most recent reports include 'SQL Injection in /api' (Triaged), 'XSS on Login Page' (Unresolved), and 'Broken Auth' (Resolved).

---

**👤 You:**
> "Create a new submission titled 'Insecure Direct Object Reference' for program prog_123."

**🤖 AI Agent:**
> Submission 'Insecure Direct Object Reference' has been successfully created for program prog_123 with ID sub_99283.


## ❓ FAQ

**Q: Can I check the scope of a security program using the agent?**
Yes! Use the `get_program` tool with the Program ID. Your agent will fetch the detailed metadata, including targets and scope descriptions, from Bugcrowd.

**Q: How do I list all the vulnerability submissions for my account?**
Simply ask the agent to `list_submissions`. It will retrieve the latest vulnerability reports from your Bugcrowd account, including titles and statuses like 'triaged' or 'resolved'.

**Q: Does the integration allow creating a new submission?**
Yes. Use the `create_submission` action and provide the title and description. You can also associate it with a specific program by providing the `program_id`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugcrowd](https://vinkius.com/mcp/bugcrowd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bugcrowd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bugcrowd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bugcrowd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bugcrowd": {
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
