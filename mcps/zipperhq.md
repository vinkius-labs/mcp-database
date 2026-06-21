# zipperHQ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zipperhq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage procurement and vendor relationships with purchase order tracking, approval workflows, and spend visibility for teams.

## Description
Connect your **zipperHQ** account to any AI agent and take full control of your video email orchestration and automated personalized messaging through natural conversation.

### What you can do

- **Video Portfolio Orchestration** — List and manage your entire high-fidelity portfolio of video emails programmatically, retrieving detailed technical metadata and SKU IDs
- **Recording & Status Intelligence** — Programmatically monitor real-time recording statuses (Pending, Uploaded, Ready) to maintain a perfectly coordinated content pipeline
- **Engagement Monitoring** — Access real-time status updates for video views (e.g., 'Last Viewed') and track individual recipient interaction directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity video durations and session IDs to maintain a perfectly coordinated media record
- **Operational Monitoring** — Verify account-level API connectivity and monitor video orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your zipperHQ dashboard (Settings > API)
3. Start orchestrating your video growth from Claude, Cursor, or any MCP client

No more manual checking of individual view counts or missing video recording status. Your AI acts as your dedicated video coordinator and messaging architect.

### Who is this for?

- **Sales Managers** — instantly retrieve video performance recaps and monitor lead interaction using natural language commands
- **Customer Success Leads** — verify individual video metadata and track client engagement history without leaving your creative workspace
- **Developers** — integrate high-speed zipperHQ video data into custom CRM and email workflows through simple AI queries


## Available Tools (10)
- **check_zipper_status**: Verify ZipperHQ API connectivity
- **get_contact_views**: Get video views for a specific contact
- **get_account**: Get your ZipperHQ account info
- **get_video_analytics**: Get analytics for a specific video
- **get_video**: Get details of a specific video
- **list_contacts**: List all video recipients
- **list_recordings**: List all screen recordings
- **list_videos**: List all video emails
- **get_recent_videos**: Get the 10 most recent videos
- **search_videos**: Search videos by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **zipperHQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all video emails sent today in my zipperHQ account."

**🤖 AI Agent:**
> I've retrieved your video emails. You currently have 5 high-fidelity transmissions today, including 'Welcome Message' for 'John Doe'. Would you like the detailed engagement metadata for any of them?

---

**👤 You:**
> "Show the view duration for the last video sent to 'Acme Corp'."

**🤖 AI Agent:**
> Engagement intelligence orchestrated! For Acme Corp, I've verified that the high-fidelity video was watched for 2:30 (90% completion). I've retrieved the technical session metadata for your review. Need help drafting a follow-up email?

---

**👤 You:**
> "Check for any video emails with 'Pending' recording status."

**🤖 AI Agent:**
> Recording architecture orchestrated! I've identified 2 high-fidelity video emails currently in 'Pending' status, including 'Contract Update' for 'Jane Client'. I've retrieved the technical session IDs for your review. Shall I notify the team to complete these recordings?


## ❓ FAQ

**Q: How do I find my zipperHQ API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I check video recording status via AI?**
Yes! The `list_videos` tool allows your agent to retrieve status metadata for all your video emails.

**Q: How do I list my sent videos?**
Use the `list_videos` tool to retrieve your complete video directory along with the unique identifiers for all managed assets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zipperhq](https://vinkius.com/mcp/zipperhq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **zipperHQ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zipperhq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **zipperHQ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zipperhq": {
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
