# Hiro.fm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hirofm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Create and distribute audio content with a podcast-like platform that lets you build a private audio feed for your audience.

## Description
Connect your **Hiro.fm** creator account to any AI agent and take full control of your private podcasting workflows through natural conversation.

### What you can do

- **Listener Management** — Create new contacts and manage your listener database with direct access to profiles and metadata
- **Access Control** — Programmatically grant or revoke access to specific private shows for any contact in your database
- **Content Automation** — Add new audio episodes to your shows by providing titles and direct media URLs directly through your agent
- **Show Monitoring** — List all your private podcast shows and retrieve detailed metadata including subscriber counts and IDs
- **Tagging & Segmentation** — Manage contact tags to organize your audience for targeted content delivery and automation

### How it works

1. Subscribe to this server
2. Enter your Hiro.fm API Key from your Creator Settings (Integrations tab)
3. Start managing your audio platform and listeners from Claude, Cursor, or any MCP client

No more manual access management or episode uploading through complex dashboards. Your AI acts as your dedicated podcast producer.

### Who is this for?

- **Course Creators** — automatically grant access to audio lessons immediately after purchase or user action
- **Membership Owners** — manage exclusive podcast feeds for your community tiers without leaving your workspace
- **Marketing Teams** — deliver personalized audio experiences and track listener engagement through automated reporting


## Available Tools (10)
- **add_audio**: Add a new audio episode
- **create_contact**: Create a new contact
- **get_contact**: Get contact details
- **get_show**: Get show details
- **grant_access**: Grant access to a show
- **list_audio**: List audio episodes for a show
- **list_contacts**: fm account.

List all contacts (listeners)
- **list_shows**: List all podcast shows
- **list_tags**: List all contact tags
- **revoke_access**: Revoke access from a show


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hiro.fm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my podcast shows from Hiro.fm."

**🤖 AI Agent:**
> I've retrieved your private shows. You currently have 3 active podcasts: 'Elite Coaching' (ID: sh_1), 'Daily Briefs' (ID: sh_2), and 'Masterclass' (ID: sh_3). Which one would you like to manage?

---

**👤 You:**
> "Grant listener access for 'john@example.com' to the 'Elite Coaching' show."

**🤖 AI Agent:**
> Access granted! John (ID: con_99) can now listen to 'Elite Coaching'. They will receive an automated email with instructions on how to access their private feed immediately.

---

**👤 You:**
> "Add a new episode titled 'Welcome Session' to my show ID 'sh_1'."

**🤖 AI Agent:**
> Episode 'Welcome Session' has been successfully added to your show. Your listeners will be able to stream it through their private feed immediately.


## ❓ FAQ

**Q: How do I get my Hiro.fm API Key?**
Log in to your Hiro.fm creator account, navigate to **Creator Settings** > **Integrations**, and copy your Bearer Token.

**Q: Can I grant access to multiple shows?**
Yes, you can use the `grant_access` tool multiple times for different `show_id` values to give a contact access to several podcasts.

**Q: Does it support adding audio from URLs?**
Yes, the `add_audio` tool requires a direct media URL to the audio file you want to add as a new episode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hirofm](https://vinkius.com/mcp/hirofm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hiro.fm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hirofm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hiro.fm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hirofm": {
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
