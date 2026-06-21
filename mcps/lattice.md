# Lattice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lattice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Retrieve HR employees, goals, feedback, and reviews directly from Lattice.

## Description
Connect your AI agent directly to **Lattice HR**. With this server, your LLM can fetch detailed employee profiles, active OKRs, tasks, and search continuous feedback loops directly tied to the Lattice platform.

### What you can do

- **Employee Directory:** Fetch user metadata directly from your HRIS via Lattice.
- **Goal Tracking:** Query active company or individual OKRs and assess progress.
- **Feedback & Praise:** Monitor continuous feedback loops and recognition events.
- **Review Cycles:** Check past and current performance review structural data.

### How it works

1. Subscribe to this endpoint
2. Enter your Lattice API token securely
3. Engage your HR tools from your development environment

### Who is this for?

- **HR Business Partners** — pull performance data effortlessly in seconds
- **Team Leads** — check team OKRs directly without context switching
- **Engineering Managers** — read feedback forms right in the IDE


## Available Tools
- **get_feedback**: Get details about a specific feedback entry
- **get_goal**: Get targeted details for a specific goal
- **get_review**: Get details regarding a specific review cycle
- **get_user**: Get details for a specific Lattice employee
- **list_feedback**: Retrieve a list of feedback and praise instances
- **list_goals**: Retrieve a list of all OKRs & Goals
- **list_reviews**: Retrieve a list of performance review cycles
- **list_tasks**: Retrieve pending tasks
- **list_users**: Retrieve a list of employees/users from Lattice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lattice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the current engineering OKRs mapped within Lattice."

**🤖 AI Agent:**
> Scanning Lattice OKRs... Found 3 goals tracked to the engineering unit focusing on Backend uptime.

---

**👤 You:**
> "Retrieve the full team employee directory for the Marketing division."

**🤖 AI Agent:**
> Sure. I fetched 12 employees logged within the Marketing division currently active.

---

**👤 You:**
> "Who received recent public praise and continuous feedback this week?"

**🤖 AI Agent:**
> Auditing recent praise... 4 instances of continuous feedback logged. The top mention highlights Sarah for her release deployment.


## ❓ FAQ

**Q: How do I authenticate?**
You need a Lattice API Key configured via Admin settings, passed into the plugin's configuration.

**Q: Can I update OKRs from this server?**
Currently the server is heavily optimized for reading OKRs, directories, and feedback.

**Q: Is employee personal data secure?**
Yes, queries route directly from your Vurb client strictly and securely into the Lattice native endpoints. Nothing is stored intermediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lattice](https://vinkius.com/mcp/lattice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lattice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lattice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lattice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lattice": {
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
