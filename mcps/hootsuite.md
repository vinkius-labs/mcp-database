# Hootsuite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hootsuite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Schedule and publish social media content, monitor brand mentions, and measure ROI across all your channels from one dashboard.

## Description
Connect your **Hootsuite** account to any AI agent and take full control of your social media presence through natural conversation.

### What you can do

- **Social Orchestration** — List and monitor all your connected social media profiles (Twitter, Facebook, LinkedIn, Instagram) in one place
- **Message Automation** — Programmatically send or schedule messages to multiple social networks simultaneously with precision
- **Content Pipeline** — Monitor outbound message history and track scheduled posts to dynamically adjust your social calendar
- **Media Management** — Create upload URLs to facilitate automated posting of rich image and video content across platforms
- **Organization Insights** — Retrieve detailed team and organization structures to manage collaborative social workflows

### How it works

1. Subscribe to this server
2. Visit the Hootsuite Developer Portal and register a new application
3. Obtain your OAuth 2.0 Access Token and paste it into the field below
4. Start managing your social networks from Claude, Cursor, or any MCP client

No more manual posting across different tabs. Your AI acts as your dedicated social media manager, ensuring consistent branding and engagement.

### Who is this for?

- **Social Media Managers** — automate repetitive posting tasks and monitor multiple profiles through a single AI interface
- **Marketing Agencies** — orchestrate client social presences and retrieve status reports using natural language
- **Content Creators** — schedule threads and posts across all platforms without leaving your creative workspace


## Available Tools
- **create_media_upload**: Requires the file size in bytes and the correct MIME type (e.g., image/jpeg or video/mp4).

Generate a media upload URL
- **create_message**: Requires the message text and a list of target social profile IDs. Optional: scheduledSendTime in ISO 8601 format.

Send or schedule a new social media message
- **delete_scheduled_message**: Requires the unique message ID obtained from outbound lists.

Delete a scheduled message
- **get_social_profile**: Includes network type, account name, and connectivity status.

Get details for a specific social profile
- **list_organization_members**: Includes member names, emails, and roles within that organization.

List members within an organization
- **list_organizations**: Organizations serve as the primary administrative unit for managing teams and social profiles.

List all Hootsuite organizations
- **list_outbound_messages**: Useful for monitoring sent posts or reviewing upcoming scheduled content.

Retrieve a list of outbound messages
- **list_social_profiles**: ) that the authenticated member has permission to manage. This is required to obtain profile IDs for scheduling messages.

List all accessible social profiles
- **list_organization_teams**: Teams are used to group members and social profiles for collaborative management.

List teams within an organization
- **get_member_info**: Use this to verify the identity and permissions of the current user.

Retrieve current Hootsuite member details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hootsuite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social media profiles in Hootsuite."

**🤖 AI Agent:**
> I've retrieved your profiles. You have 4 networks connected: Twitter (@TechCorp), Facebook Page (TechCorp Official), LinkedIn (TechCorp), and Instagram (@TechCorp_Life). Which one should we use for your next post?

---

**👤 You:**
> "Schedule a post with text 'Excited for our product launch!' for tomorrow at 10 AM."

**🤖 AI Agent:**
> Message scheduled! I've set your post for tomorrow at 10:00 AM across Twitter and LinkedIn. You can track it in your scheduled messages history.

---

**👤 You:**
> "Check my outbound messages for the last 24 hours."

**🤖 AI Agent:**
> Scanning history... In the last 24 hours, you've sent 3 messages: 2 on Twitter and 1 on Facebook. All were delivered successfully with no errors reported.


## ❓ FAQ

**Q: How do I find social profile IDs?**
You can use the `list_social_profiles` tool to retrieve a list of all connected social networks and their unique IDs.

**Q: Can I schedule posts for multiple profiles at once?**
Yes, the `create_message` tool accepts a comma-separated list of profile IDs to post or schedule to multiple networks simultaneously.

**Q: What is the correct time format for scheduling?**
You should use the ISO 8601 format (e.g., 2026-04-18T10:00:00Z) for the `scheduledSendTime` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hootsuite](https://vinkius.com/mcp/hootsuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hootsuite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hootsuite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hootsuite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hootsuite": {
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
