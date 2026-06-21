# Digify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digify-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Share documents securely with dynamic watermarks, access controls, and analytics that show exactly who viewed each page.

## Description
Connect your **Digify** account to any AI agent and take full control of your secure document distribution and Virtual Data Room (VDR) workflows through natural conversation.

### What you can do

- **Document Protection Orchestration** — Programmatically protect sensitive files with granular Digital Rights Management (DRM) settings, including view-only access and dynamic watermarks
- **VDR Architecture** — Create and manage secure Virtual Data Rooms for high-stakes business collaboration, including inviting guests and managing folder structures
- **Engagement Intelligence** — Retrieve detailed audit logs and activity reports to monitor who accessed your protected documents and for how long
- **Access Control Lifecycle** — Programmatically revoke access or update sharing permissions for individual files or entire Data Rooms directly through your agent
- **Administrative Visibility** — Monitor Data Room engagement statistics and manage webhook configurations to maintain a high-fidelity secure ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Key ID** and **Key Secret** from your Digify Developer dashboard
3. Start securing your corporate assets from Claude, Cursor, or any MCP client

No more manual watermarking or complex invitation tracking in the web portal. Your AI acts as your dedicated security and document operations coordinator.

### Who is this for?

- **Legal & Finance Teams** — instantly secure sensitive contracts and manage M&A Data Rooms using natural language commands
- **Corporate Executives** — track engagement with confidential board materials and board books without leaving your workspace
- **Operations Leads** — automate guest provisioning and monitor audit trails through simple AI queries


## Available Tools
- **create_dataroom**: Create a new Data Room
- **get_account_info**: Get account status
- **get_dataroom_stats**: Get Data Room engagement stats
- **get_dataroom**: Get Data Room details
- **get_file**: Get file details
- **invite_guest**: Invite a guest to a Data Room
- **list_activities**: Track document activities
- **list_datarooms**: List Virtual Data Rooms
- **list_files**: List protected files
- **list_dataroom_guests**: List Data Room participants
- **list_webhooks**: List configured webhooks
- **protect_file**: Securely share a file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Virtual Data Rooms in my account."

**🤖 AI Agent:**
> I've retrieved your secure environments. You currently have 3 active Data Rooms: 'Project Phoenix' (M&A), 'Board Materials 2026', and 'Investor Due Diligence'. Which one should I list the guests for?

---

**👤 You:**
> "Securely share 'Q1_Financials.pdf' with 'john.doe@example.com' (no download allowed)."

**🤖 AI Agent:**
> File protected! I've generated a secure sharing link for 'Q1_Financials.pdf' with view-only permissions for John Doe. The link is: [secure_url]. I'll notify you as soon as they access the file.

---

**👤 You:**
> "Show the last 5 activities for the 'Project Phoenix' Data Room."

**🤖 AI Agent:**
> Fetching audit logs... The last 5 events include: @user1 viewed 'Asset_List.xlsx', @user2 downloaded the 'NDA', and 3 new guest invitations. Would you like the detailed timestamps for these activities?


## ❓ FAQ

**Q: How do I find my Digify Key ID and Secret?**
Log in to your account at [digify.com](https://digify.com/), navigate to the **API** section in your dashboard, and generate a new set of API keys.

**Q: Can I prevent recipients from downloading protected files?**
Yes! The `protect_file` tool includes an `allow_download` parameter. Set it to `false` to enable view-only access via the secure link.

**Q: How do I invite multiple guests to a Data Room?**
Use the `invite_guest` tool for each participant. You can ask your agent to process a list of emails to coordinate batch invitations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digify-alternative](https://vinkius.com/mcp/digify-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `digify-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digify-alternative": {
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
