# Plane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plane)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage Plane.so projects, track issues, review sprint cycles, and audit agile modules completely autonomously.

## Description
Equip any AI agent with direct access to your **Plane** workspace. Whether you're using Plane Cloud or self-hosting, your AI assistant can seamlessly retrieve projects, analyze agile cycles, and parse the active issues pipeline without forcing you to click through kanban boards manually.

### What you can do

- **Projects & Core Entities** — Extract isolated project architectures spanning across your Workspace, pulling high-fidelity descriptions and status parameters.
- **Agile Cycles (Sprints)** — Command the agent to list and structure your active development cycles, evaluating timelines and completion statuses.
- **Work Items (Issues)** — Perform deep sweeps over tasks and explicit tickets inside boundary states, analyzing what your engineering team is actually building.
- **Modules & Taxonomy** — Read epics (modules) and static categorization labels dictating your issue pipelines.

### How it works

1. Install this integration onto your agent layer
2. Provide your Plane Personal API Key (and optionally, your self-hosted API URL)
3. Start fetching sprints and active cycles immediately from Cursor, Claude, or any MCP client

### Who is this for?

- **Project Managers** — instantly retrieve all pending tasks in the current cycle (`list_cycles` & `list_work_items`) and summarize progress dynamically.
- **Lead Engineers** — inspect the ticket backlog without leaving your IDE; write code and verify module requirements consecutively.
- **Product Teams** — cross-reference structured modules versus labels without dealing with the visual planner interface.


## Available Tools (6)
- **list_cycles**: List cycles inside a Plane project
- **list_modules**: List modules inside a Plane project
- **list_labels**: List project labels in Plane
- **list_projects**: List projects in a Plane workspace
- **get_project**: Get specific details of a Plane project
- **list_work_items**: List work items (issues) inside a Plane project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all cross-functional modules targeting project `project-x`."

**🤖 AI Agent:**
> Pinging standard workspace schemas... I matched Project 'Frontend Rewrite'. There are 4 distinct modules attached: `Auth Module`, `Kanban Redesign`, `API Rate Limiter`, and `User Onboarding`. Looking at `Auth Module`, it is targeting completion by October 20th. Do you need its related tags?

---

**👤 You:**
> "Are there any pending work items left in the current active active sprint?"

**🤖 AI Agent:**
> Looking at cycle `v1.2 Release`, I've pulled 4 unresolved work items out of the 15 originally mapped. Ticket `ID: 9912` (Database Race Condition) is holding up priority, currently marked 'In Progress' by the QA tag. Want me to investigate its raw configuration?

---

**👤 You:**
> "Fetch the exact details of the issue designated ID `3841-A` on the board."

**🤖 AI Agent:**
> Extracted the data entity mapped to `3841-A`. Title: `Handle missing env parameters explicitly during build steps`. It carries the labels 'High Priority' and 'DevOps'. The raw issue content requests adding an abort sequence checking for missing variables natively during CI initialization. How would you like me to script this?


## ❓ FAQ

**Q: Can my AI automatically aggregate all open issues inside our active sprint?**
Yes. First, request the active iteration window by calling `list_cycles`. The agent will isolate today's active cycle bounds. Following that, it will invoke `list_work_items` directly constrained by that cycle object, outputting an exhaustive summary of untouched or blocking tickets.

**Q: How does the agent handle custom workspace slugs or self-hosted URLs?**
The system dynamically accepts a `PLANE_BASE_URL` credential. If you are doing an on-premise installation running inside your homelab or company AWS cloud, you merely inject your private domain (e.g., `https://plane.internal.acme.com`). The workspace slug is seamlessly accepted as a contextual execution parameter during standard query prompts.

**Q: Can I request specific details of a long-term module (epic)?**
You can instruct the agent to execute `list_modules`. It extracts the cross-functional epics spanning your workspace project. Your AI can read these top-level module architectures to contextually understand what the core functionality of the project repository aims to achieve.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plane](https://vinkius.com/mcp/plane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plane": {
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
