# FusionSignage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusionsignage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Control digital signage screens remotely with content scheduling, playlist management, and real-time display monitoring.

## Description
Connect your **FusionSignage** account to any AI agent and manage your digital signage network through natural conversation.

### What you can do

- **Screen Management** — List all screens with online/offline status, inspect configurations, update settings, and check real-time connectivity
- **Playlist Builder** — Create, update, and delete content playlists with media items and display order
- **Content Assignment** — Assign playlists to specific screens for targeted content delivery
- **Media Library** — Browse all uploaded media (images, videos, web pages), inspect file metadata, and remove outdated assets
- **Content Scheduling** — Create time-based schedules with playlist rotation and screen assignments
- **Screen Groups** — Organize screens into groups for bulk content management

### How it works

1. Subscribe to this server
2. Enter your FusionSignage API Key from your account settings
3. Start managing your signage network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Facility Managers** — monitor screen status, push content updates, and manage display groups without accessing the dashboard
- **Marketing Teams** — schedule campaigns, rotate promotional content, and update digital menus through AI
- **IT Administrators** — audit screen connectivity, manage media libraries, and troubleshoot display issues


## Available Tools (17)
- **assign_playlist**: Assign playlist to screen
- **check_fusion_status**: Verify connectivity
- **create_playlist**: Create a playlist
- **create_schedule**: Create a schedule
- **delete_media**: Delete media
- **delete_playlist**: Delete a playlist
- **get_media_item**: Get media details
- **get_playlist**: Get playlist details
- **get_screen_status**: Get screen status
- **get_screen**: Get screen details
- **list_groups**: List screen groups
- **list_media**: List all media
- **list_playlists**: List all playlists
- **list_schedules**: List schedules
- **list_screens**: List all screens
- **update_playlist**: Update a playlist
- **update_screen**: Update a screen


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FusionSignage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all screens and highlight any that are offline."

**🤖 AI Agent:**
> Your signage network has 12 screens. 10 online, 2 offline. ⚠️ Offline screens: 1) 'Lobby Display' (screen_003, last seen 2 hours ago, assigned: 'Welcome Playlist'). 2) 'Cafeteria Menu' (screen_008, last seen 45 min ago, assigned: 'Lunch Menu'). Online screens include: 'Reception TV' (screen_001, playing 'Corporate News'), 'Meeting Room A' (screen_002, playing 'Room Schedule'), and 8 others. Would you like to update the offline screen configurations or assign new playlists?

---

**👤 You:**
> "Create a new promotional playlist with our latest media and assign it to all lobby screens."

**🤖 AI Agent:**
> Media library: 34 files available. Latest uploads: 'spring_promo_2025.mp4' (15s, uploaded today), 'new_menu_banner.jpg', 'loyalty_program.mp4' (30s). Playlist created! ID: pl_892, Name: 'Spring Promo 2025', Items: 3 media files, Total duration: 55s loop. Assigned to 3 lobby screens: 'Lobby Display' (screen_003), 'Lobby Left' (screen_004), 'Lobby Right' (screen_005). All screens will update within 60 seconds. Would you like to create a schedule or update the playlist?

---

**👤 You:**
> "Show all content schedules and the screen groups configured in our account."

**🤖 AI Agent:**
> Active schedules: 4. 1) 'Business Hours' — Mon-Fri 8AM-6PM, plays 'Corporate News' on all lobby screens. 2) 'Lunch Menu' — Mon-Fri 11AM-2PM, plays 'Daily Menu' on cafeteria screens. 3) 'Weekend Mode' — Sat-Sun all day, plays 'Welcome Loop' on reception. 4) 'After Hours' — Mon-Fri 6PM-8AM, plays 'Security Info' on all screens. Screen groups: 1) 'Lobby' (3 screens). 2) 'Cafeteria' (2 screens). 3) 'Meeting Rooms' (5 screens). 4) 'External' (2 screens). Would you like to create a new schedule or modify a group?


## ❓ FAQ

**Q: Can I monitor which screens are online or offline in real time?**
Yes. Use `list_screens` to see all screens with their current online/offline status and assigned content. For a specific screen, use `get_screen_status` to check real-time connectivity and playback status. Use `get_screen` for detailed configuration including orientation and playlist assignment.

**Q: Can I create a playlist and assign it to a screen?**
Yes. Use `create_playlist` with a JSON payload containing name and media items. Then use `assign_playlist` with the screen ID and playlist ID to push it to a display. Use `update_playlist` to modify content order or add new media, and `delete_playlist` to remove unused playlists.

**Q: Can I schedule content to play at specific times?**
Yes. The `create_schedule` tool accepts a JSON configuration with time slots, playlist rotations, and screen assignments. Use `list_schedules` to view all active schedules. Combine with `list_groups` to manage multiple screens simultaneously through group assignments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusionsignage](https://vinkius.com/mcp/fusionsignage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FusionSignage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fusionsignage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FusionSignage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fusionsignage": {
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
