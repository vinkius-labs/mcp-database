# Hootsuite (Social Media Management) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hootsuite-social-media-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hootsuite-social-media-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hootsuite-social-media-management-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Hootsuite (Social Media Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hootsuite-social-media-management](https://vinkius.com/mcp/hootsuite-social-media-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
