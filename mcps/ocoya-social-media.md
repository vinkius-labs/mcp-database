# Ocoya Social Media MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ocoya-social-media)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage Ocoya social profiles, posts, workspaces, and workflows.

## Description
# Ocoya

The Ocoya MCP Server allows AI agents to interact with your social media management platform seamlessly.

### What you can do
- Retrieve user workspaces and profiles.
- Access scheduled and published posts.
- View active automations and workflows.

### How it works
Connect your Ocoya account via your API Key to manage your social media marketing data remotely.


## Available Tools (9)
- **get_automation**: Get a specific automation/workflow
- **get_me**: Get current authenticated user info
- **get_post**: Get a specific post
- **get_profile**: Get a specific social profile
- **get_workspace**: Get a specific workspace
- **list_automations**: List all automations/workflows
- **list_posts**: List all posts
- **list_profiles**: List all social profiles
- **list_workspaces**: List all workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ocoya Social Media** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve all my scheduled marketing posts for the Black Friday campaign running on my Ocoya workspace."

**🤖 AI Agent:**
> I've retrieved your scheduled posts. You have 4 upcoming posts for the Black Friday campaign, including '50% Off Sitewide Announcement' set for Twitter and 'Midnight Flash Sale' queued for LinkedIn. Would you like me to pause any of these?

---

**👤 You:**
> "Check which social media profiles are currently connected and active in my main Ocoya workspace."

**🤖 AI Agent:**
> I found 3 active social profiles connected to your workspace: '@VinkiusLabs' (Twitter), 'Vinkius Official' (LinkedIn Company Page), and 'Vinkius Design' (Instagram Business). The connection status for all 3 is currently healthy.

---

**👤 You:**
> "Show me all active marketing workflows and automations running in my Ocoya account right now."

**🤖 AI Agent:**
> I found 3 active automations in your Ocoya account: 'Blog to Twitter Sync', 'Weekly Newsletter Promo', and 'Instagram Story Cross-post'. All triggers are functioning normally. Would you like to view the execution history of a specific workflow?


## ❓ FAQ

**Q: Where do I find my API Key?**
Your API Key can be generated in the Ocoya Developer or Integrations settings page.

**Q: What access does this MCP need?**
It requires your API Key to access your profiles, workspaces, and posts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ocoya-social-media](https://vinkius.com/mcp/ocoya-social-media)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ocoya Social Media** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ocoya-social-media` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ocoya Social Media** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ocoya-social-media": {
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
