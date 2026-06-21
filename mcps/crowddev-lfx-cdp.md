# crowd.dev (LFX CDP) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowddev-lfx-cdp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crowddev-lfx-cdp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crowddev-lfx-cdp-mcp)
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


## Installation & Usage

To install and use the **crowd.dev (LFX CDP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowddev-lfx-cdp](https://vinkius.com/mcp/crowddev-lfx-cdp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
