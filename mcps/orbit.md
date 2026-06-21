# Orbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage community relationships via Orbit — list members, track activities, and add notes directly from any AI agent.

## Description
Connect your **Orbit** workspace to any AI agent and take full control of your community management and engagement workflows through natural conversation.

### What you can do

- **Member Oversight** — List all community members and retrieve detailed profiles, including social links and reach metrics.
- **Activity Tracking** — Monitor the timeline of activities across your workspace and create new activities for members.
- **Organization Discovery** — List and retrieve details for organizations associated with your community members.
- **Relationship Management** — List and create notes on member profiles to maintain context on your interactions.
- **Engagement Insights** — Fetch a detailed history of activities for any specific member to understand their journey.

### How it works

1. Subscribe to this server
2. Enter your Orbit API Key and Workspace ID
3. Start managing your community directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Community Managers** — quickly check a member's activity history or add a note after a meaningful interaction.
- **Developer Relations (DevRel)** — track contributions and engagement across GitHub, Twitter, and other platforms.
- **Marketing Teams** — monitor the growth and activity levels of specific community segments through simple queries.




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 members who joined our community."

**🤖 AI Agent:**
> I've retrieved the latest members. Some recent additions include 'Alice Dev', 'Tech Enthusiast', and 'Growth Hacker'. Would you like their full profiles?

---

**👤 You:**
> "Show me the activity history for member 'john_doe'."

**🤖 AI Agent:**
> John Doe has been quite active! In the last 30 days, he has posted 3 tweets, attended 1 webinar, and submitted 2 PRs on GitHub.

---

**👤 You:**
> "Add a note to member 98765 saying 'Had a great call today about their upcoming blog post'."

**🤖 AI Agent:**
> The note has been successfully added to member 98765's profile. It will be visible to your team in Orbit.


## ❓ FAQ

**Q: How do I find my Orbit API Key?**
In your Orbit account, go to **Settings** > **Account Settings**. Your API token is listed in the 'API Token' section.

**Q: Where is the Workspace ID located?**
The Workspace ID is the unique slug found in the URL of your Orbit dashboard (e.g., `app.orbit.love/YOUR_WORKSPACE_ID`).

**Q: Can I add custom activities for members?**
Yes! Use the `create_orbit_activity` tool. You can specify the `activity_type` and provide a link or unique key to record any community interaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orbit](https://vinkius.com/mcp/orbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `orbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orbit": {
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
