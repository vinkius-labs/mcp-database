# BlackTwist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blacktwist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Enrich B2B lead data with verified company information, technographics, and contact details for precision targeting.

## Description
Connect your **BlackTwist** account to any AI agent and take full control of your social media presence on **Threads** and **Bluesky** through natural conversation.

### What you can do

- **Post & Thread Orchestration** — Draft and schedule high-fidelity posts or entire threads to your connected accounts programmatically in real-time
- **Advanced Analytics Intelligence** — Retrieve detailed engagement metrics, monitor posting consistency, and access high-fidelity daily performance recaps
- **Provider Management Architecture** — List and manage your connected social media providers and coordinate your digital voice across multiple profiles
- **Automated Audience Growth** — Access and monitor auto-plug templates and follow-up settings to perfectly coordinate your brand's growth strategy
- **Infrastructure Monitoring** — Access your current subscription status, post quotas, and account settings directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your BlackTwist dashboard (Settings > API)
3. Start orchestrating your social media growth from Claude, Cursor, or any MCP client

No more manual toggling between social apps or digging through analytics dashboards. Your AI acts as your dedicated social media manager and content architect.

### Who is this for?

- **Content Creators** — instantly schedule threads and analyze performance using natural language commands
- **Social Media Managers** — manage multiple Threads and Bluesky accounts without leaving your creative workspace
- **Growth Leads** — monitor engagement trends and automate follow-up strategies through simple AI queries


## Available Tools (12)
- **create_post**: You must specify the providerId and the content of the post(s).

Create or schedule a new post
- **delete_post**: If it was scheduled, it will be cancelled.

Delete a post
- **get_posting_consistency**: Get posting consistency data
- **get_daily_recap**: Get yesterday’s activity summary
- **get_thread_follow_up**: Get follow-up settings for a thread
- **get_analytics_metrics**: ) for your social media accounts.

Get engagement metrics
- **get_post**: Get details for a specific post
- **get_account_settings**: Get account settings
- **get_subscription_info**: Get current plan and quota
- **list_posts**: List your posts and drafts
- **list_accounts**: Useful for getting providerIds.

List connected social media accounts
- **list_follow_up_templates**: List auto-plug/follow-up templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlackTwist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all social media accounts connected to BlackTwist."

**🤖 AI Agent:**
> I've retrieved your social profiles. You currently have a Threads account (@user1, ID: 123) and a Bluesky account (ID: 456) connected. Which one should we use for a new post?

---

**👤 You:**
> "Schedule a Threads post 'Check out our new API!' for tomorrow at 2 PM."

**🤖 AI Agent:**
> Post scheduled! I've successfully queued your update 'Check out our new API!' on Threads for tomorrow at 2:00 PM. The run ID is 'post_789'. Shall I monitor the engagement once it's live?

---

**👤 You:**
> "Show my engagement metrics and daily activity recap."

**🤖 AI Agent:**
> Accessing analytics... Yesterday you reached 1,500 views and 120 likes across all accounts. Your consistency score is holding at 98%. Would you like the detailed breakdown per profile?


## ❓ FAQ

**Q: How do I find my BlackTwist API Key?**
Log in to your account, navigate to **Settings** > **API**, and click **Generate New API Key** to get your token.

**Q: Can I schedule threads with media?**
The current toolset is optimized for text-based post and thread orchestration to maintain high-fidelity engagement.

**Q: How do I check my remaining post quota?**
Use the `get_subscription_info` tool to retrieve your current plan details and remaining publication credits directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blacktwist](https://vinkius.com/mcp/blacktwist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlackTwist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blacktwist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlackTwist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blacktwist": {
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
