# Targetprocess MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/targetprocess)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to Apptio Targetprocess. Agile portfolio management natively from the terminal: track user stories, active bugs, and sprint iterations seamlessly.

## Description
Empower your conversational matrix with enterprise Agile planning tools by establishing a secure MCP bridge to **Apptio Targetprocess**. Stop navigating cumbersome management web panels during your deep work sessions. Allow your LLM to function as your personal Scrum Master, parsing detailed product backlogs, pinpointing active bugs, and analyzing sprint iterations entirely from within your prompt. Unify your engineering tasks by having constant programmatic awareness of your organization's roadmap execution.

### What you can do

- **Project & Portfolio Mapping** — Request high-level structured arrays defining active scopes natively operating `list_projects` and view associated global product `list_features`.
- **Sprint & Iteration Sync** — Track time-bound execution containers seamlessly querying `list_iterations` to understand immediate team commitments.
- **Backlog & Requirements Auditing** — Read explicit product developments dispatching analytical traces executing `list_user_stories` to capture detailed requirement specs.
- **Defect Discovery** — Swiftly analyze current technical debts monitoring live system anomalies by interrogating `list_bugs` without leaving your IDE.

### How it works

1. Append the Targetprocess connective configuration module logic safely inside your Vinkius environment.
2. Bind your designated organizational host `TP_ACCOUNT` alongside your private authorization string `TP_ACCESS_TOKEN` exported securely from your Targetprocess Settings.
3. Prompt Agile intelligence contextually: "Show me the active issues tracked in our main project, identify what sprint iteration we are in, and fetch the top three user stories assigned."

### Who is this for?

- **Engineering Team Leads** — Effortlessly audit defect queues (`list_bugs`) and sync sprint scopes (`list_iterations`) dynamically during active code reviews.
- **Agile Product Owners** — Extrapolate explicit organizational `list_features` hierarchies validating requirements textually bypassing graphical interface friction.
- **Release Management Specialists** — Formally invoke deep structural readouts analyzing user story progression and mapping global projects cleanly over the terminal.


## Available Tools
- **list_bugs**: Lists reported bugs/defects
- **list_features**: Lists high-level features (capabilities)
- **list_iterations**: Lists iterations (sprints)
- **list_projects**: Lists all projects in Targetprocess
- **list_user_stories**: Lists user stories in the account
- **list_account_users**: Lists all registered users in the Targetprocess account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Targetprocess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the current active Sprint iterations and pull the details of the top 3 unassigned bugs logged under our primary development project."

**🤖 AI Agent:**
> Gathering structural records ('list_iterations')...
Evaluating active Sprint: 'Iteration Q4-B'.
Now querying current technical debts via 'list_bugs'...

**Found Top Defects**:
- Bug-145: 'Memory leak in auth parser' (Critical)
- Bug-199: 'Missing CSS button radius' (Medium)
- Bug-231: 'Gateway timeout during 2FA' (High)

---

**👤 You:**
> "Extract the details for user story #4552 in the current sprint."

**🤖 AI Agent:**
> Interrogating agile entities ('get_entity_details')...
User Story #4552: 'Implement SSO Auth'
- State: In Progress
- Assigned to: Alice B.
- Story Points: 5
- Iteration: Sprint 14

---

**👤 You:**
> "List all high priority bugs that are currently 'Open'."

**🤖 AI Agent:**
> Querying Targetprocess data ('search_entities')...
I found 2 'Open' bugs tagged with High Priority:
1. Bug #5120: 'Payment gateway timeout in production'
2. Bug #5125: 'Null pointer exception on invoice generation'


## ❓ FAQ

**Q: Is the integration read-only?**
Yes. All tools (list_projects, list_bugs, list_user_stories, etc.) are read-only queries. They cannot modify, create, or delete any records in Targetprocess.

**Q: Where do I find my access token?**
Go to Settings > Access Tokens in your Targetprocess instance. Generate a new token and copy it. You'll also need your account subdomain (e.g., `mycompany` from `mycompany.tpondemand.com`).

**Q: What agile data can the agent access?**
Projects, features, user stories, bugs, iterations (sprints), and team members. The scope depends on the permissions of the access token you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/targetprocess](https://vinkius.com/mcp/targetprocess)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Targetprocess** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `targetprocess` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Targetprocess** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "targetprocess": {
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
