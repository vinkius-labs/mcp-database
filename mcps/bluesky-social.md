# Bluesky Social MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bluesky-social)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Publish posts, follow accounts, and engage with the decentralized social network through your AI-powered workflow.

## Description
Connect your **Bluesky** account to any AI agent and take full control of your decentralized social interactions and automated microblogging workflows through natural conversation.

### What you can do

- **Microblogging Orchestration** — Publish high-fidelity posts to your Bluesky profile programmatically with automatic link and mention detection in real-time
- **Relationship Intelligence** — Manage your social graph by following/unfollowing accounts and retrieving detailed high-fidelity follower/following directories
- **Search & Profile Discovery** — Access complete profile metadata, bios, and statistics for any handle or DID to coordinate your organizational social research
- **Timeline & Feed Monitoring** — Monitor your home timeline and notifications programmatically to maintain high-fidelity oversight of your social engagement
- **Moderation Architecture** — Programmatically mute or unmute actors and discover trending custom feed generators to perfectly coordinate your digital feed experience

### How it works

1. Subscribe to this server
2. Retrieve your **Handle** (e.g., name.bsky.social) and generate an **App Password** in Bluesky settings (Settings > App Passwords)
3. Start orchestrating your decentralized social presence from Claude, Cursor, or any MCP client

No more manual toggling between social apps or missing important mentions in the feed. Your AI acts as your dedicated social media manager and AT Protocol architect.

### Who is this for?

- **Social Media Managers** — instantly publish updates and monitor community feedback using natural language commands
- **Developers & Power Users** — automate the management of decentralized social connections without leaving your workspace
- **Researchers** — analyze trending feeds and search for influence patterns through simple AI queries


## Available Tools (12)
- **follow_user**: Follow an account
- **list_muted_users**: List muted users
- **list_notifications**: Get notifications
- **list_timeline**: Get your home feed
- **get_profile**: Get user profile
- **list_popular_feeds**: List popular feed generators
- **list_followers**: List account followers
- **create_post**: Post to Bluesky
- **get_user_posts**: List user posts
- **mute_user**: Mute an account
- **search_profiles**: Search for users
- **unmute_user**: Unmute an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bluesky Social** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Post to Bluesky: 'Enjoying the new decentralized web experience!'"

**🤖 AI Agent:**
> Post published successfully! Your update is now live on your Bluesky profile. I've enabled automatic link detection for you. Shall I monitor for any immediate replies?

---

**👤 You:**
> "Show the last 5 posts in my home timeline."

**🤖 AI Agent:**
> Retrieving timeline... Your home feed features 5 recent posts, including a tech update from @user1 and several community discussions. Would you like the detailed author metadata for any of these?

---

**👤 You:**
> "Search for users interested in 'MCP Servers' and show their profiles."

**🤖 AI Agent:**
> Searching social graph... I found 3 users matching your query, including 'Vinkius' and 2 other tech profiles. I've retrieved their high-fidelity bios and follower counts for you. Shall I follow any of them?


## ❓ FAQ

**Q: How do I find my Bluesky Handle and App Password?**
Your handle is your username (e.g., name.bsky.social). For the password, go to **Settings** > **App Passwords** in Bluesky and generate a new one.

**Q: Can I search for users via AI?**
Yes! The `search_profiles` tool allows your agent to find Bluesky users matching a text query programmatically.

**Q: How do I check my social notifications?**
Use the `list_notifications` tool to retrieve recent likes, reposts, and mentions directly through your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bluesky-social](https://vinkius.com/mcp/bluesky-social)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bluesky Social** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bluesky-social` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bluesky Social** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bluesky-social": {
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
