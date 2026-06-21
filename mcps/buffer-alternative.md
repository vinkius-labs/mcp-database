# Buffer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buffer-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan, schedule, and publish social media content across all your channels with analytics that show what is working.

## Description
Connect your **Buffer** account to any AI agent and take full control of your social media strategy and automated content distribution through natural conversation.

### What you can do

- **Profile Orchestration** — List and manage all connected social media profiles (Twitter, Facebook, LinkedIn, etc.) programmatically, retrieving detailed metadata and follower statistics
- **Content Lifecycle Management** — Programmatically schedule new posts (updates) across multiple platforms in real-time, including support for media links and high-fidelity text content
- **Queue & History Intelligence** — Monitor your pending post queue and retrieve detailed historical records of successfully published updates to maintain a consistent online presence
- **Engagement Architecture** — Access real-time engagement statistics for specific posts to coordinate your social media performance and ROI directly through your agent
- **Schedule Optimization** — Access and monitor your posting times and frequency rules to perfectly coordinate your brand's digital voice programmatically

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from your Buffer account (Settings > Personal Access Tokens)
3. Start planning your social media growth from Claude, Cursor, or any MCP client

No more manual toggling between different social platforms or digging through fragmented post histories. Your AI acts as your dedicated social media manager and content architect.

### Who is this for?

- **Social Media Managers** — instantly retrieve post performance and schedule cross-platform updates using natural language commands
- **Digital Marketers** — automate content distribution and monitor brand engagement without leaving your workspace
- **Developers** — integrate high-speed social media automation into custom marketing workflows through simple AI queries


## Available Tools
- **schedule_social_post**: Schedule a new post
- **remove_social_post**: Delete a post
- **modify_pending_post**: Edit scheduled post
- **get_api_status**: Check connection
- **list_pending_posts**: Check scheduled queue
- **get_profile_details**: Get account info
- **get_posting_schedules**: Check posting times
- **list_published_posts**: Check post history
- **get_post_details**: Get post info
- **list_social_profiles**: ) connected to Buffer.

List connected accounts
- **test_buffer_auth**: Verify credentials
- **modify_posting_schedules**: Set posting times


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buffer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my connected social media profiles in Buffer."

**🤖 AI Agent:**
> I've retrieved your social profiles. You currently have 3 connected accounts: Twitter (@user1), LinkedIn (ID: abc), and Facebook Page. Which one should we manage or check for scheduled posts?

---

**👤 You:**
> "Schedule a post: 'Excited to announce our new integration!' for Twitter and LinkedIn profiles."

**🤖 AI Agent:**
> Content scheduled! I've successfully added your update to the queue for both Twitter and LinkedIn. It will be published according to your next available time slot. Shall I check your current posting schedule?

---

**👤 You:**
> "Show the engagement statistics for my last 5 published posts."

**🤖 AI Agent:**
> Fetching historical performance... Your last 5 posts received a total of 1,240 impressions and 85 clicks. Your post from yesterday was the top performer with a 5% engagement rate. Would you like the detailed metadata for it?


## ❓ FAQ

**Q: How do I find my Buffer Access Token?**
Log in to your Buffer account, navigate to **Settings** > **Personal Access Tokens**, and generate a new token for your integration.

**Q: Can I post to multiple social profiles at once?**
Yes! The `schedule_social_post` tool accepts a JSON array of profile IDs, allowing you to broadcast the same update across all your connected platforms.

**Q: How do I check my scheduled queue?**
Use the `list_pending_posts` tool with a specific profile ID to retrieve all updates currently waiting to be published.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buffer-alternative](https://vinkius.com/mcp/buffer-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buffer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `buffer-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buffer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buffer-alternative": {
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
