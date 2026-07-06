# Text In Church MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/text-in-church)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Keep your congregation engaged with church-specific texting, email, and communication tools that grow attendance and giving.

## Description
Connect your **Text In Church** account to any AI agent and simplify how you manage your congregation directory, volunteer groups, and community outreach through natural conversation.

### What you can do

- **Member Management** — List all church people and visitors, and add new members to your directory programmatically.
- **Group Oversight** — List church groups, volunteer lists, and ministries to keep your community organized.
- **SMS Outreach** — Send text messages to entire groups or specific individuals directly via AI commands.
- **Keyword Tracking** — List active keywords used for automated sign-ups and visitor responses.
- **Visitor Engagement** — Log new visitors and manage their contact data to ensure timely follow-ups.
- **Communication Visibility** — Monitor your outreach campaigns and group memberships directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Text In Church API Key (found in your developer settings)
3. Start managing your church communications from Claude, Cursor, or any MCP client

### Who is this for?

- **Church Administrators** — quickly retrieve member lists and coordinate group announcements via simple AI queries.
- **Pastors & Ministry Leads** — send encouragement messages and verify visitor data directly from the workspace.
- **Volunteer Coordinators** — manage team groups and automate follow-ups with new members via the AI assistant.


## Available Tools (5)
- **send_church_sms**: Send an SMS message
- **add_church_person**: Add a new person
- **list_church_groups**: List church groups
- **list_church_keywords**: List active keywords
- **list_church_people**: List people in the church directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Text In Church** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active groups in my church account."

**🤖 AI Agent:**
> I've retrieved your groups. You have 5 active communities: 'Sunday Volunteers', 'Youth Group', 'New Members', 'Finance Committee', and 'Community Outreach'. Which one would you like to send a message to?

---

**👤 You:**
> "Send an SMS to the 'Sunday Volunteers' group: 'Reminder: Briefing at 8:00 AM tomorrow'."

**🤖 AI Agent:**
> Message sent! I've triggered the SMS alert to all members of the 'Sunday Volunteers' group. Every volunteer should receive the reminder shortly.

---

**👤 You:**
> "Search for a member named 'Sarah Smith' in the directory."

**🤖 AI Agent:**
> I've found the record. Sarah Smith (ID: p_10293) is a registered member. She is part of the 'Youth Group' and her last interaction was 2 days ago. Shall I retrieve her full contact details?


## ❓ FAQ

**Q: Can I send an SMS to a specific group using the AI?**
Yes! Use the `send_church_sms` tool and provide the Group ID and your message content. Your agent will trigger the broadcast to all members of that group instantly.

**Q: How do I see all the active keywords for my church?**
Run the `list_church_keywords` query. The agent will retrieve a complete list of keywords configured in your account for automated responses and sign-ups.

**Q: Is it possible to add a new visitor via AI?**
Absolutely. Use the `add_church_person` action. Provide the first name, last name, and contact details (phone/email) to instantly register the new visitor in your directory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/text-in-church](https://vinkius.com/mcp/text-in-church)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Text In Church** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `text-in-church` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Text In Church** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "text-in-church": {
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
