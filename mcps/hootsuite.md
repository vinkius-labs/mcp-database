# Hootsuite MCP Server

Schedule and publish social media content, monitor brand mentions, and measure ROI across all your channels from one dashboard.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hootsuite)

## Overview
**Category:** growth-engine
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Hootsuite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hootsuite](https://vinkius.com/mcp/hootsuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
