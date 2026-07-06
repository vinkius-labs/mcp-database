# NationBuilder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nationbuilder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Organize communities, run campaigns, and mobilize supporters with a platform built for political and nonprofit leadership.

## Description
Connect your **NationBuilder** account to any AI agent and take full control of your community orchestration and campaign mobilization through natural conversation. NationBuilder is the leading software for political campaigns and non-profits, and this integration allows you to retrieve signup metadata, record donations, and monitor petition engagement directly from your chat interface.

### What you can do

- **Signup & Audience Orchestration** — List all managed signups and retrieve detailed profile metadata programmatically to ensure your voter or donor database is always synchronized.
- **Donation Lifecycle Management** — Record and monitor financial contributions directly from the AI interface to track campaign fundraising goals.
- **Petition & Advocacy Intelligence** — Access and monitor active petitions and retrieve supporter metadata via natural language to drive better mobilization efficiency.
- **Community Tagging Control** — List and search through your nation's tags and custom people lists to maintain a clear overview of your segments using simple AI commands.
- **Operational Monitoring** — Track system responses and manage event metadata to ensure your campaign workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your NationBuilder Access Token (v2) and Nation Slug from your control panel
3. Start managing your nation from Claude, Cursor, or any MCP-compatible client

No more manual data entry for single donations or supporter checks. Your AI acts as a dedicated campaign manager or community coordinator.

### Who is this for?

- **Campaign Managers** — quickly retrieve supporter summaries and monitor donation trends without switching apps.
- **Non-profit Organizers** — automate the recording of donations and track petition growth via natural conversation.
- **Developers** — integrate real-time community data and supporter metadata directly within the chat.


## Available Tools (12)
- **get_signup_details**: Get person info
- **list_recent_donations**: List contributions
- **list_upcoming_events**: List calendar events
- **list_custom_people_lists**: List curated lists
- **list_nation_petitions**: List active petitions
- **list_nation_signups**: List people/signups
- **list_nation_sites**: List CMS sites
- **list_signup_tags**: List available tags
- **find_signup_by_email**: Find person
- **record_donation**: Add donation record
- **create_new_signup**: Add new person
- **get_api_status**: Check connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NationBuilder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 signups in my nation."

**🤖 AI Agent:**
> I've retrieved your recent signups. You have 5 new supporters including 'Robert Chen' and 'Alice Miller'. Would you like to see the tags for any of them?

---

**👤 You:**
> "Show me all upcoming events scheduled in my nation."

**🤖 AI Agent:**
> I found 3 upcoming events in your nation. "Town Hall Meeting" is scheduled for May 15th with 42 RSVPs, "Volunteer Training" on May 20th has 18 confirmed attendees, and "Community Fundraiser" on June 1st has 89 RSVPs so far.

---

**👤 You:**
> "Find the person with email john.smith@example.com in my database."

**🤖 AI Agent:**
> Found a match. John Smith (ID: 8342) is a registered supporter since March 2024. He has the tags "volunteer" and "donor", with 2 recorded donations totaling $150. His current status is "active supporter".


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific signup by their email?**
Yes! Use the `search_signups` tool. Provide the email address, and your agent will respond with complete metadata for the profile, including tags and unique ID in seconds.

**Q: How do I find my Nation Slug?**
The Nation Slug is the unique prefix in your NationBuilder URL (e.g., if you log in at `mynation.nationbuilder.com`, your slug is `mynation`).

**Q: Does this support the NationBuilder API v2?**
Yes, this MCP server is built specifically for the NationBuilder REST API v2, utilizing the modern JSON:API specification for all data interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nationbuilder](https://vinkius.com/mcp/nationbuilder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NationBuilder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nationbuilder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NationBuilder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nationbuilder": {
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
