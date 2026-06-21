# Autobidder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autobidder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Optimize your ad spend with AI-powered bidding strategies that automatically adjust bids across advertising platforms.

## Description
Connect your **Autobidder** account to any AI agent and take full control of your project bidding orchestration and automated response workflows through natural conversation.

### What you can do

- **Bid Portfolio Orchestration** — List and manage all incoming bid requests and tenders programmatically, retrieving detailed technical metadata
- **Response & Quote Intelligence** — Programmatically query and monitor active project bids to maintain a perfectly coordinated revenue overview
- **Win Rate Architecture** — Access your complete directory of past bids and outcomes to oversee your organizational performance in real-time
- **Deadline Monitoring** — Access real-time status updates for bid deadlines and track submission progress directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor bid orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Autobidder dashboard (Settings > API)
3. Start orchestrating your project growth from Claude, Cursor, or any MCP client

No more manual checking of tender portals or missing bid deadlines. Your AI acts as your dedicated bidding coordinator and project architect.

### Who is this for?

- **Estimators & Bidding Managers** — instantly retrieve bid summaries and monitor submission goals using natural language commands
- **Business Development Leads** — verify individual project metadata and track win history without leaving your creative workspace
- **Developers** — integrate high-speed Autobidder data into custom internal tools through simple AI queries


## Available Tools
- **check_autobidder_status**: Verify AutoBidder API connectivity
- **create_request**: Create a bid request
- **get_bid**: Get bid details
- **get_outcome**: Get outcome details
- **get_profile**: Get your profile
- **get_request**: Get request details
- **list_bids**: List all bids
- **list_outcomes**: List all bid outcomes
- **list_projects**: List all projects
- **list_requests**: List all bid requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Autobidder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active bid requests in my Autobidder account."

**🤖 AI Agent:**
> I've retrieved your requests. You currently have 15 active tender profiles, including 'Project A' and 'Tender B'. Would you like the detailed technical metadata for any of them?

---

**👤 You:**
> "Show the win rate for 'Team Alpha' last month."

**🤖 AI Agent:**
> Bidding intelligence orchestrated! For Team Alpha, I've identified a win rate of 40% from last month's submissions. I've retrieved the project metadata for your review. Need help auditing the lost bids?

---

**👤 You:**
> "Check for any bid deadlines approaching this week."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 3 bid deadlines this week, including 'Hospital Upgrade' on Friday. I've retrieved the technical requirement metadata for your review. Shall I notify the estimators?


## ❓ FAQ

**Q: How do I find my Autobidder API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I check bid win rates via AI?**
Yes! The `list_outcomes` tool allows your agent to retrieve status metadata for all your past submissions.

**Q: How do I list my active bid requests?**
Use the `list_requests` tool to retrieve your complete directory along with the unique identifiers for all managed tenders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autobidder](https://vinkius.com/mcp/autobidder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Autobidder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `autobidder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Autobidder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autobidder": {
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
