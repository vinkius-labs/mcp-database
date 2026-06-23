# Kisi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kisi-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Control building access with cloud-managed smart locks, mobile credentials, and audit trails that replace traditional key cards.

## Description
Connect your **Kisi** account to any AI agent and take full control of your facility's physical security and high-fidelity access orchestration through natural conversation.

### What you can do

- **Lock Portfolio Orchestration** — List all cloud-connected locks, retrieve detailed high-fidelity status metadata, and monitor door health programmatically
- **Remote Unlock Operations** — Programmatically trigger high-fidelity remote unlocks for specific doors directly through your agent for perfectly coordinated visitor access
- **Facility Lockdown Architecture** — Access high-fidelity emergency lockdown protocols for individual doors or entire places to ensure immediate site security
- **Place & Site Discovery** — Access your complete directory of high-fidelity physical locations and places to understand and orchestrate your facility infrastructure
- **User & Member Monitoring** — List organization users and access complete high-fidelity profile metadata to maintain perfect security alignment
- **Operational Monitoring** — Verify account-level API connectivity and monitor access orchestration volume directly through your agent for perfectly coordinated security scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Kisi dashboard (Settings > API Keys)
3. Start managing your facility security from Claude, Cursor, or any MCP client

No more manual checking of individual door logs or physical keycards. Your AI acts as your dedicated security coordinator and facility architect.

### Who is this for?

- **Security Managers** — instantly retrieve lock statuses and monitor site health using natural language commands without leaving your creative workspace
- **Facility Managers** — trigger high-fidelity remote unlocks and monitor door activity to ensure healthy and secure operations
- **IT Admins** — verify technical API logs and user assignments to optimize access control through simple AI queries


## Available Tools (10)
- **get_kisi_lock**: Get lock details
- **get_kisi_place**: Get place details
- **get_kisi_user**: Get user details
- **list_kisi_groups**: List access groups
- **lockdown_kisi_lock**: Lockdown a door
- **list_kisi_locks**: List cloud locks
- **list_kisi_places**: List physical places
- **check_kisi_status**: Check API Status
- **unlock_kisi_lock**: Unlock a door
- **list_kisi_users**: List organization users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kisi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all cloud locks and show their current status."

**🤖 AI Agent:**
> I've retrieved your locks. You currently have 12 active high-fidelity doors, including 'Front Entrance' (Online) and 'Server Room' (Locked). Would you like to see the detailed health metadata for any of them?

---

**👤 You:**
> "Unlock the 'Front Entrance' door for 10 seconds."

**🤖 AI Agent:**
> Access orchestrated! I've triggered a high-fidelity remote unlock for 'Front Entrance' (ID: lock_123) for a duration of 10 seconds. Your security connection is healthy. Shall I monitor the activity log for this door?

---

**👤 You:**
> "Check the team members in the 'HQ Office' place."

**🤖 AI Agent:**
> Facility directory orchestrated! The 'HQ Office' place currently has 45 high-fidelity profiles assigned. Your API connection is healthy. Shall I retrieve the detailed resource access metadata for this site?


## ❓ FAQ

**Q: How do I find my Kisi API Key?**
Log in to your account, navigate to **Settings** > **API Keys**, and generate a new high-fidelity **API Secret**.

**Q: Can I unlock a door via AI?**
Yes! The `unlock_kisi_lock` tool allows your agent to trigger a high-fidelity remote unlock for any cloud-connected door in your organization.

**Q: How do I list my organization's places?**
Use the `list_kisi_places` tool to retrieve the complete high-fidelity directory of physical locations along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kisi-alternative](https://vinkius.com/mcp/kisi-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kisi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kisi-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kisi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kisi-alternative": {
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
