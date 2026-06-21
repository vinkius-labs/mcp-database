# crowd.dev (LFX CDP) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowddev-lfx-cdp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Equip your AI agent to manage community members, activities, and organizations directly via the crowd.dev (LFX) API.

## Description
Integrate **crowd.dev** (now part of the Linux Foundation as the **LFX Community Data Platform**), the comprehensive community data and orchestration platform, directly into your AI workflow. Monitor community growth, track member activities across multiple platforms, and manage your community CRM using natural language.

### What you can do

- **Member Management** — List, search, and retrieve full profiles and activity history for community members.
- **Activity Tracking** — Monitor real-time community engagement (stars, messages, commits) across different platforms.
- **Organization Insights** — Explore companies and organizations associated with your community members.
- **Community CRM** — Manage internal notes and tasks to optimize your community management workflows.

### How it works

1. Connect the crowd.dev integration to your AI assistant.
2. Authorize using your crowd.dev API Key (found in your dashboard Settings).
3. Manage your community data and engagement strategy through intuitive conversation.

### Who is this for?

- **Community Managers** — Quickly identify key contributors and track engagement trends.
- **Developer Advocates** — Audit activities across GitHub, Discord, and Slack via chat.
- **Marketing Teams** — Explore organization-level data to understand community composition.


## Available Tools
- **create_community_member**: Touches identity management and profile initialization boundaries.

Register a new member in the community
- **get_community_health_summary**: Resolves new member growth, activity volume trends, and platform distribution stats.

Get a high-level summary of community activities and growth
- **get_member_details**: Touches engagement scoring, social identity resolution, and community role boundaries.

Get full profile and activity history for a specific member
- **get_organization_details**: Touches firmographic details and aggregate contribution metrics boundary.

Get details for a specific organization
- **list_recent_activities**: Resolves activity types (e.g., star, PR, message), associated platforms, and member references.

List recent community activities (stars, messages, etc.)
- **list_members**: dev community platform. Resolves member names, social profiles (GitHub, LinkedIn, Twitter), and contribution activity levels.

List all community members in crowd.dev
- **list_member_notes**: Resolves note content, author ID, and associated community member links.

List internal CRM notes for community members
- **list_organizations**: Resolves company names, domains, and the number of employees active in the community.

List companies and organizations in your community
- **list_community_tasks**: Resolves task descriptions, priority levels, and assigned community manager references.

List open tasks related to community management
- **search_members_by_keyword**: Resolves member profiles matching the specified name or email criteria.

Search for community members by name or email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **crowd.dev (LFX CDP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all community members who have been active in the last 7 days."

**🤖 AI Agent:**
> I've retrieved 45 members who were active this week. Top contributors include 'jdoe', 'dev_advocate', and 'user123'. Would you like to see their recent activities?

---

**👤 You:**
> "Show me the details for community member 'jdoe'."

**🤖 AI Agent:**
> Member 'jdoe' has an engagement score of 85. They are active on GitHub and Discord, with 12 contributions this month. Their primary organization is 'TechCorp'. Should I list their internal notes?

---

**👤 You:**
> "List all organizations associated with our community members."

**🤖 AI Agent:**
> I've found 15 organizations associated with your members, including 'Google', 'Red Hat', and 'Vinkius'. 'Red Hat' has the highest number of active contributors. Would you like a detailed report?


## ❓ FAQ

**Q: How do I get a crowd.dev API Key?**
Log in to your crowd.dev (or LFX CDP) dashboard, navigate to **Settings > API Keys**, and generate a new key. Copy and paste it below.

**Q: Which platforms are supported for activity tracking?**
crowd.dev supports integration with major platforms including GitHub, Discord, Slack, LinkedIn, Twitter, and more to provide a unified view of your community.

**Q: Can I update member profiles via chat?**
Currently, the integration focuses on listing and retrieving member data. For bulk updates or complex profile management, please use the crowd.dev dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowddev-lfx-cdp](https://vinkius.com/mcp/crowddev-lfx-cdp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **crowd.dev (LFX CDP)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `crowddev-lfx-cdp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **crowd.dev (LFX CDP)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crowddev-lfx-cdp": {
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
