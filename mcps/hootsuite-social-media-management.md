# Hootsuite (Social Media Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hootsuite-social-media-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage social media via Hootsuite — schedule posts, manage social profiles, and monitor outbound messages.

## Description
Connect your **Hootsuite** account to any AI agent and take full control of your enterprise social media management and content scheduling through natural conversation.

### What you can do

- **Content Scheduling** — Draft and schedule messages across multiple social networks simultaneously, including precise timing and timezone management directly from your agent
- **Social Profile CRM** — List and inspect all connected social profiles (Twitter, Facebook, Instagram, LinkedIn) and retrieve detailed network metadata
- **Message Management** — Monitor outbound message queues within specific time ranges and selectively delete scheduled content before it goes live
- **Media Orchestration** — Handle high-throughput media uploads with presigned cloud URLs and monitor processing states for images and videos
- **Organization Audit** — Navigate across different Hootsuite organizations and list registered team members and roles to manage collaborative workflows securely

### How it works

1. Subscribe to this server
2. Enter your Hootsuite OAuth Access Token
3. Start managing your social presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — schedule weekly content and monitor outbound queues through natural conversation without jumping between tabs
- **Marketing Operations** — audit team member roles and organization structures across multiple social media properties
- **Agency Leads** — manage content for multiple clients by switching between social profiles and organization boundaries efficiently


## Available Tools (10)
- **list_social_profiles**: List all connected social profiles
- **get_media_upload_url**: Get a media upload URL
- **get_social_profile**: Get social profile details
- **list_messages**: List scheduled and sent messages
- **create_message**: Optionally schedule for a future time (ISO 8601).

Schedule a social media post
- **delete_message**: Delete a scheduled message
- **list_organizations**: List all organizations
- **list_teams**: List teams in an organization
- **list_members**: List organization members
- **get_me**: Get authenticated user info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hootsuite (Social Media Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social profiles connected to Hootsuite"

**🤖 AI Agent:**
> I've found 4 connected social profiles: 'TechCorp_Twitter' (ID: 123), 'TechCorp_LinkedIn' (ID: 456), 'Personal_IG' (ID: 789), and 'Facebook_Page' (ID: 012). Which one would you like to use for your next post?

---

**👤 You:**
> "Schedule a post for tomorrow at 10 AM: 'Excited to announce our new product launch! #innovation'"

**🤖 AI Agent:**
> Scheduling post… I've set your message to be published tomorrow at 10:00 AM across Twitter and LinkedIn. The Message ID is msg-98765. Would you like to check the media upload status if you attached an image?

---

**👤 You:**
> "What messages are scheduled to go out today?"

**🤖 AI Agent:**
> I've retrieved 3 scheduled messages for today: 'Q2 Roadmap Highlights' (2 PM), 'Customer Spotlight' (4 PM), and 'Industry News' (6 PM). Would you like to see the full text or social profiles for any of these?


## ❓ FAQ

**Q: Can I schedule a post for multiple social networks at once?**
Yes. The `schedule_message` tool accepts an array of social profile IDs. Your agent can send the same text content to all selected networks (e.g. Twitter and LinkedIn) in a single command, ensuring cross-platform consistency.

**Q: How do I find the ID of a social profile?**
Ask your agent to `list_social_profiles`. It will return all connected accounts along with their unique IDs, network type (TWITTER, FACEBOOK, etc.), and usernames, making it easy to identify the correct target for your posts.

**Q: Can I delete a scheduled post if I find an error?**
Absolutely. Use the `delete_message` tool with the specific Message ID. Your agent will remove the pending post from the Hootsuite queue, preventing it from being published.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hootsuite-social-media-management](https://vinkius.com/mcp/hootsuite-social-media-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hootsuite (Social Media Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hootsuite-social-media-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hootsuite (Social Media Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hootsuite-social-media-management": {
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
