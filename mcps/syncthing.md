# Syncthing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/syncthing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage file synchronization via Syncthing — monitor device connections, browse directories, and control sync folders directly from any AI agent.

## Description
Connect your **Syncthing** instance to any AI agent and take full control of your private file synchronization infrastructure through natural conversation.

### What you can do

- **Device Monitoring** — List all configured devices and check their real-time connection status and metadata.
- **Folder Management** — Query all synchronized folders, check their database status, and monitor completion percentages.
- **System Control** — Pause or resume synchronization for specific devices, restart the Syncthing process, or check if a configuration change requires a restart.
- **Directory Browsing** — Remotely list directories matching specific paths to verify file structures across your sync network.
- **Configuration & Stats** — Fetch or update the entire system configuration and retrieve detailed statistics for folders and devices.

### How it works

1. Subscribe to this server
2. Enter your Syncthing Web UI URL and API Key
3. Start managing your P2P sync network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sysadmins & DevOps** — monitor distributed sync nodes and manage configurations without leaving the terminal or chat interface.
- **Power Users** — check the health of home lab backups and trigger folder scans or device resumes via voice or text.
- **Data Managers** — verify that specific files have synced across the network by browsing remote directories through the AI.


## Available Tools (28)
- **system_browse**: List directories matching a path
- **system_connections**: Get configured devices and connection status
- **get_db_completion**: Get folder/device completion status
- **get_db_file**: Get detailed data about a specific file
- **scan_db**: Request immediate scan of a folder
- **get_db_status**: ).

Get folder database status
- **get_device_stats**: Get device statistics
- **get_events**: Poll for events
- **get_folder_stats**: Get folder statistics
- **get_config**: Get entire configuration
- **get_db_ignores**: Get ignore patterns for a folder
- **get_device**: Get specific device configuration
- **get_devices**: Get all configured devices
- **get_folder**: Get specific folder configuration
- **get_folders**: Get all configured folders
- **get_health**: Returns {"status": "OK"}. Does not require authentication.

Simple health check
- **system_pause**: If device ID is omitted, affects all devices.

Pause devices
- **get_random_string**: Get a strong random alphanumeric string
- **system_reset**: Optionally reset only a specific folder.

Reset index database
- **get_restart_required**: Check if restart is required
- **system_restart**: Restart Syncthing
- **system_resume**: If device ID is omitted, affects all devices.

Resume devices
- **set_config**: Replace entire configuration
- **set_db_ignores**: Set ignore patterns for a folder
- **system_shutdown**: Shutdown Syncthing
- **system_status**: ).

Get current system status and resource usage
- **verify_device_id**: Verify and format a device ID
- **system_version**: Get Syncthing version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Syncthing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all connected devices and their current status."

**🤖 AI Agent:**
> I've retrieved the connection status. You have 3 devices configured: 'Laptop-Main' (Connected), 'Backup-NAS' (Connected), and 'Phone-Sync' (Disconnected).

---

**👤 You:**
> "Check the system status and resource usage of my Syncthing instance."

**🤖 AI Agent:**
> The system is healthy. Uptime is 48 hours, memory usage is 156MB, and the current version is v1.27.2. No restart is currently required.

---

**👤 You:**
> "List the directories inside the path '/data/backups/photos'."

**🤖 AI Agent:**
> Browsing the path... I found 3 subdirectories: '2023-Vacation', 'Family-Events', and 'Work-Archive'.


## ❓ FAQ

**Q: How can I check if Syncthing needs a restart after I changed the configuration?**
You can use the `get_restart_required` tool. It will return a boolean indicating if a restart is pending due to configuration changes.

**Q: Is it possible to pause synchronization for a specific device using the AI?**
Yes. Use the `system_pause` tool and provide the specific Device ID. If you omit the ID, it will pause all devices.

**Q: Can I see which files are currently being synchronized?**
You can use `get_db_status` or `get_db_completion` for a specific folder to see the synchronization progress and state of the files in that directory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/syncthing](https://vinkius.com/mcp/syncthing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Syncthing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `syncthing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Syncthing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "syncthing": {
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
