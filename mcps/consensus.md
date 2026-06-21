# CONSENSUS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/consensus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Share interactive product demos with prospects that track engagement and reveal which features matter most to each buyer.

## Description
Connect your **Consensus** account to any AI agent and take full control of your interactive video demo and buyer intelligence workflows through natural conversation.

### What you can do

- **DemoBoard Orchestration** — List and manage your active DemoBoards programmatically, retrieving detailed metadata about leads and stakeholder engagement
- **Demolytics Intelligence** — Access real-time analytics to understand which sections of your automated demos are being watched, skipped, or shared by prospects
- **Invitation Tracking** — Programmatically monitor sent demo invitations and track outreach performance to coordinate perfectly timed sales follow-ups
- **Asset Discovery** — Retrieve a complete directory of all available interactive demos and assets in your library to maintain high-fidelity sales enablement
- **Team Visibility** — Access directories of account users and roles to maintain an organized sales team structure and permission oversight

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Secret** from Consensus (Settings > Integrations > API Credentials)
3. Start managing your interactive sales pipeline from Claude, Cursor, or any MCP client

No more manual status checking of individual demo links. Your AI acts as your dedicated sales associate and demolytics coordinator.

### Who is this for?

- **Sales SDRs & AEs** — instantly retrieve lead engagement summaries and monitor who is watching your demos using natural language commands
- **Sales Operations** — track overall demo performance and team usage metrics without leaving your communication tools
- **Marketing Leads** — monitor interactive asset popularity and buyer intent signals through simple AI queries


## Available Tools
- **get_demoboard**: Get DemoBoard details
- **list_demoboards**: List all DemoBoards
- **list_demolytics**: List analytics for demos
- **list_demos**: List all available demos
- **list_invitations**: List sent demo invitations
- **list_users**: List all account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CONSENSUS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active DemoBoards in Consensus."

**🤖 AI Agent:**
> I've retrieved your DemoBoards. You currently have 5 active boards, including 'Q2 Tech Prospect' (ID: db_123) and 'Enterprise SaaS 2026'. Which one would you like to see lead data for?

---

**👤 You:**
> "Show me the Demolytics summary for my latest demo."

**🤖 AI Agent:**
> Fetching analytics... Your latest demo has 150 total views with an average engagement score of 85%. Viewers are spending the most time on the 'Cloud Security' feature. Shall I check for any new invitations?

---

**👤 You:**
> "List all members of my sales team and their roles."

**🤖 AI Agent:**
> I've retrieved your team directory. You have 8 members: 2 Admins, 5 Sales Reps (User), and 1 Analyst. Would you like the individual activity logs for any team member?


## ❓ FAQ

**Q: How do I find my Consensus API Key and Secret?**
Log in to your account, navigate to **Settings** > **Integrations** > **API Credentials**, and generate a new set of keys.

**Q: What are Demolytics?**
Demolytics provide deep insights into buyer engagement, showing exactly which parts of your interactive demos were most valuable to a prospect.

**Q: Can I see all invitations sent via AI?**
Yes! Use the `list_invitations` tool to retrieve a complete history of demo invites sent from your account programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/consensus](https://vinkius.com/mcp/consensus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CONSENSUS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `consensus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CONSENSUS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "consensus": {
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
