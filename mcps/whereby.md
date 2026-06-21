# Whereby MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whereby)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whereby-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whereby-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Create video meeting rooms, manage recordings, and customize UI themes on Whereby — the easiest way to embed video calls.

## Description
Connect your **Whereby** account to any AI agent and manage your video communication infrastructure through natural conversation.

### What you can do

- **Meeting Creation** — Instantly provision new transient video meeting rooms with specific expiration dates and room modes (normal or group)
- **Meeting Insights** — Retrieve full details for any meeting, including the exact join URL and real-time status
- **UI Customization** — Update and manage visual room themes, including custom colors and branding, to match your application's look and feel
- **Recording Management** — List all cloud recordings stored in your account and retrieve direct MP4 download links and metadata
- **Active Sessions** — Monitor currently active or pending meeting rooms and retrieve their unique UUIDs for automated workflows
- **Data Integrity** — Safely delete obsolete meeting rooms or cloud recordings to manage your quotas and storage efficiently
- **Room Controls** — Configure room security by setting rooms to 'locked' mode, requiring host approval for new participants

### How it works

1. Subscribe to this server
2. Enter your Whereby API Key
3. Start managing your video rooms and recordings through Claude, Cursor, or any MCP-compatible client

No more manual navigation through meeting dashboards to create a room. Your AI agent becomes your video operations assistant.

### Who is this for?

- **Product Developers** — test meeting creation and UI theme customization for embedded video applications
- **Operations Teams** — automate room provisioning for customer calls and manage cloud recording storage
- **Support Engineers** — quickly create secure, transient rooms for troubleshooting sessions through chat
- **Marketing Managers** — audit meeting recordings and verify room branding for webinars and events


## Available Tools
- **create_meeting_room**: Provide an ISO 8601 end date and room mode (normal or group).

Creates a new transient video meeting room with a specific end date
- **delete_meeting_room**: This action is irreversible.

Immediately deletes a video meeting room and terminates any active session
- **delete_cloud_recording**: This action is irreversible.

Permanently deletes a cloud recording file
- **reset_room_theme**: Resets a meeting room theme back to the default Whereby branding
- **get_meeting_details**: Retrieves details for a specific video meeting, including its join URL and expiration date
- **get_recording_details**: Retrieves download links and metadata for a specific cloud recording
- **get_room_theme**: Retrieves the visual theme settings (colors, logo) for a specific room name
- **list_active_meetings**: Lists all currently active or pending video meeting rooms created via the API
- **list_cloud_recordings**: Lists all cloud recordings stored in the Whereby account
- **update_room_theme**: Provide the room name and a hex color code.

Updates the primary branding color for a specific meeting room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Whereby** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new 'group' meeting room that expires in 2 hours."

**🤖 AI Agent:**
> I've created a new group meeting room. It is set to expire on 2026-04-01 at 12:00 PM UTC. Your join URL is: https://whereby.com/room-abc-123. Would you like me to lock the room as well?

---

**👤 You:**
> "List all my past cloud recordings."

**🤖 AI Agent:**
> I found 3 recordings: 1. 'Project Sync' (2026-03-25), 2. 'Client Demo' (2026-03-28), and 3. 'Strategy Session' (2026-03-30). Would you like the download link for any of these?

---

**👤 You:**
> "Update the 'Support-101' room theme to use hex color #00ff00."

**🤖 AI Agent:**
> Successfully updated the theme for room 'Support-101'. The primary branding color is now set to #00ff00 (Green). You can view the changes in your embedded iframe immediately.


## Installation & Usage

To install and use the **Whereby** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whereby](https://vinkius.com/mcp/whereby)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
