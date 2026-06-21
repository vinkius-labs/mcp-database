# Phabricator (Development Platform Conduit API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phabricator-development-platform-conduit-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage tasks, code reviews, and repositories via Phabricator's Conduit API — search Maniphest tasks, edit revisions, and query users directly.

## Description
Connect your **Phabricator** instance to any AI agent to streamline your development workflow. This server leverages the Conduit API to provide deep integration with Maniphest, Differential, and Diffusion.

### What you can do

- **Task Management (Maniphest)** — Search for tasks using complex filters, create new tasks, or update existing ones (status, owners, comments) using `maniphest_search` and `maniphest_edit`.
- **Code Reviews (Differential)** — Query and search for code revisions, or perform actions like accepting and requesting changes via `differential_revision_search` and `differential_revision_edit`.
- **Repository Insights (Diffusion)** — List and filter repositories or search for specific commits using `diffusion_repository_search` and `diffusion_commit_search`.
- **Audit History** — Retrieve the full transaction history of any task to understand its lifecycle with `maniphest_gettasktransactions`.
- **User Management** — Identify the authenticated user or search for other contributors across the platform.

### How it works

1. Subscribe to this server
2. Provide your Phabricator Instance URL and Conduit API Token
3. Start managing your monorepo and tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Software Engineers** — Check task details or update code revisions without leaving your IDE.
- **Release Managers** — Track commit history and repository status across the entire organization.
- **Project Leads** — Audit task histories and manage sprint progress through natural language queries.


## Available Tools (10)
- **differential_query**: Query Differential revisions (Legacy)
- **differential_revision_edit**: Create or update a Differential revision
- **differential_revision_search**: Search for Differential revisions
- **diffusion_commit_search**: Search for Diffusion commits
- **diffusion_repository_search**: Search for Diffusion repositories
- **maniphest_edit**: Create or update a Maniphest task
- **maniphest_gettasktransactions**: Get transaction history for a task
- **maniphest_search**: Supports complex filtering via constraints.

Search for Maniphest tasks
- **user_search**: Search for users
- **user_whoami**: Get details about the authenticated user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phabricator (Development Platform Conduit API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is the currently authenticated Phabricator user?"

**🤖 AI Agent:**
> I've checked your credentials. You are currently logged in as 'dev_lead' (PHID-USER-1234567890).

---

**👤 You:**
> "Search for all open tasks in Maniphest assigned to me."

**🤖 AI Agent:**
> I found 3 open tasks assigned to you: T452 (Fix Auth Bug), T458 (Update Documentation), and T460 (Refactor Database). Would you like more details on any of these?

---

**👤 You:**
> "Show me the recent history for task T101."

**🤖 AI Agent:**
> Retrieving history for T101... The task was created by 'alice' 2 days ago, moved to 'In Progress' by 'bob' yesterday, and 'charlie' added a comment regarding the API specs 4 hours ago.


## ❓ FAQ

**Q: Can I update the status of a Maniphest task using this server?**
Yes. You can use the `maniphest_edit` tool. You'll need to provide the task identifier (like T123) and a transaction object specifying the 'status' type and the desired value.

**Q: How do I see the full history of changes for a specific task?**
Use the `maniphest_gettasktransactions` tool with the task ID (e.g., 'T123'). It will return a chronological list of all edits, comments, and status changes made to that task.

**Q: Can I search for code revisions that are currently open?**
Absolutely. Use `differential_revision_search` and pass a constraint for statuses like 'open' or 'needs-review' to filter the results to active code reviews.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phabricator-development-platform-conduit-api](https://vinkius.com/mcp/phabricator-development-platform-conduit-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phabricator (Development Platform Conduit API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phabricator-development-platform-conduit-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phabricator (Development Platform Conduit API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phabricator-development-platform-conduit-api": {
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
