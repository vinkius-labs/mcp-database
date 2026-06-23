# Gerrit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gerrit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage code reviews via Gerrit — query changes and patch sets, handle reviewers and approvals, and audit project branches directly from any AI agent.

## Description
Connect your **Gerrit Code Review** instance to any AI agent and take full control of your collaborative code reviews, project repositories, and patch set management through natural conversation.

### What you can do

- **Change & Review Orchestration** — Query Gerrit changes using advanced syntax like 'status:open' or 'owner:self' to retrieve subjects, numbers, and owners natively
- **Patch Set Auditing** — List all revisions (patch sets) of a change to track commit SHAs, uploader info, and parent commits for detailed version history flawlessly
- **Reviewer & Approval Oversight** — Enumerate reviewers on any change and retrieve approval labels (Code-Review, Verified) to monitor the consensus process synchronousy
- **Project & Repository Navigation** — List all projects and retrieve detailed metadata including states (ACTIVE/READ_ONLY) and default branch configurations securely
- **Branch Management** — Identify and list all branches within a Gerrit project, extracting the latest commit SHAs to verify repository boundaries natively
- **Account & Identity Discovery** — Fetch authenticated user profile information and list associated verified email addresses to verify account contexts flawlessy
- **Group & Access Auditing** — List all Gerrit groups to identify who controls access to projects and grants specific permissions within your organizational tree

### How it works

1. Subscribe to this server
2. Enter your Gerrit URL, Username, and HTTP Password (found in your Gerrit Settings > HTTP Password)
3. Start managing your code reviews from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers & Maintainers** — track open changes and review patch sets without leaving the chat or IDE interface
- **Engineering Managers** — audit code review progress and verify approval labels using natural language conversation
- **DevOps Engineers** — test and debug Gerrit API integrations and verify project branch structures in real-time
- **SRE Teams** — monitor project states and verify organizational group permissions through natural conversation


## Available Tools (10)
- **query_changes**: Uses syntax: "status:open", "owner:self", "project:myproj". Returns subjects, numbers, statuses, owners, projects, patches.

Query changes (code reviews) on Gerrit
- **get_change**: Get full details of a Gerrit change
- **list_projects**: List all projects (repositories) on Gerrit
- **get_project**: Get full details of a Gerrit project
- **list_branches**: List all branches in a Gerrit project
- **get_account**: Get the authenticated Gerrit account
- **list_emails**: List all email addresses associated with the authenticated Gerrit account
- **list_reviewers**: List all reviewers on a Gerrit change
- **list_patchsets**: List all patch sets (revisions) of a Gerrit change
- **list_groups**: Returns group names, IDs, owners, and descriptions.

List all groups on Gerrit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gerrit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my open changes in project 'core-engine'"

**🤖 AI Agent:**
> Retrieving your changes... I found 2 open changes in 'core-engine': #501 'Fix memory leak' and #502 'Refactor logging'. Would you like to see the current patch set for either of these?

---

**👤 You:**
> "Who are the reviewers for change #501?"

**🤖 AI Agent:**
> Retrieving reviewers for #501... I found 3 reviewers: Alice (Code-Review: +2), Bob (Code-Review: +1), and Charlie (Verified: +1). The change is currently awaiting more approvals to be merged.

---

**👤 You:**
> "List all branches in project 'frontend-v2'"

**🤖 AI Agent:**
> Retrieving branches for 'frontend-v2'... I found 3 branches: 'master' (SHA: abc123), 'release-v1.0' (SHA: def456), and 'feature-auth'. Would you like the latest commit message for any of these?


## ❓ FAQ

**Q: Can my agent list open changes across all Gerrit projects?**
Yes. Use the 'query_changes' tool with the query 'status:open'. The agent will retrieve the global array of all matching changes, including subjects, numbers, and owners natively.

**Q: How do I see the approval labels (Code-Review, Verified) for a specific change via chat?**
Use the 'get_change' tool. It retrieves the full details of a Gerrit change, including the 'labels' section where you can see the Code-Review and Verified scores assigned by reviewers natively.

**Q: Can I check which groups have access to a specific project through the agent?**
Absolutely. Use the 'list_groups' tool to identify existing groups. While project access rules are often defined in the project settings, the agent can help you verify group definitions and ownership within your organizational tree flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gerrit](https://vinkius.com/mcp/gerrit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gerrit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gerrit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gerrit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gerrit": {
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
