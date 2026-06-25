# Hetzner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hetzner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Hetzner Cloud infrastructure—list servers, manage firewalls, and control power states directly from any AI agent.

## Description
Connect your **Hetzner Cloud** account to any AI agent to orchestrate your infrastructure through natural language.

### What you can do

- **Server Management** — List all active servers, fetch specific details, and create or delete instances on demand.
- **Power Control** — Remotely power on servers or rebuild them from specific images using simple commands.
- **Networking & Security** — Manage private networks, configure firewalls, and handle floating IPs to ensure connectivity.
- **Load Balancing** — List and create load balancers to distribute traffic across your infrastructure efficiently.

### How it works

1. Subscribe to this server
2. Enter your Hetzner Cloud API Token
3. Start managing your cloud resources from Claude, Cursor, or any MCP-compatible client

No more manual navigation through the cloud console for routine checks. Your AI acts as a cloud engineer, providing instant visibility into your VPS fleet.

### Who is this for?

- **DevOps Engineers** — quickly audit server states and firewall rules without leaving the terminal or IDE
- **System Administrators** — automate power cycles and resource monitoring through conversation
- **Developers** — spin up or rebuild development environments directly from a coding assistant


## Available Tools (38)
- **list_certificates**: List all certificates
- **create_certificate**: Create a new certificate
- **get_storage_box**: Get details of a specific Storage Box
- **list_images**: List all images
- **create_firewall**: Create a new firewall
- **create_floating_ip**: Create a new floating IP
- **create_load_balancer**: Create a new load balancer
- **create_network**: Create a new network
- **create_server**: Create a new server
- **create_ssh_key**: Create a new SSH key
- **create_storage_box_snapshot**: Create a manual snapshot for a Storage Box
- **create_storage_box_subaccount**: Create a subaccount for a Storage Box
- **create_volume**: Create a new volume
- **create_zone**: Create a new DNS zone
- **list_datacenters**: List all datacenters
- **delete_load_balancer**: Delete a load balancer
- **delete_server**: Delete a server
- **list_firewalls**: List all firewalls
- **list_floating_ips**: List all floating IPs
- **get_action**: Get details of a specific action
- **get_server**: Get details of a specific server
- **list_load_balancers**: List all load balancers
- **list_locations**: List all locations
- **list_networks**: List all networks
- **list_placement_groups**: List all placement groups
- **poweron_server**: Power on a server
- **list_primary_ips**: List all primary IPs
- **rebuild_server**: Rebuild a server from an image
- **list_server_types**: List all server types
- **list_servers**: List all servers
- **list_ssh_keys**: List all SSH keys
- **list_storage_box_snapshots**: List snapshots for a Storage Box
- **list_storage_box_subaccounts**: List subaccounts for a Storage Box
- **list_storage_boxes**: List all Storage Boxes
- **update_storage_box**: Update Storage Box settings (e.g., enable/disable protocols like SMB, WebDAV)
- **list_volumes**: List all volumes
- **list_zones**: List all DNS zones
- **list_isos**: List all ISOs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hetzner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active servers in the Hetzner Cloud."

**🤖 AI Agent:**
> I've found 3 servers: 'web-prod' (ID: 12345, running), 'db-master' (ID: 12346, running), and 'staging-app' (ID: 12347, off).

---

**👤 You:**
> "Get the full details for server ID 12345."

**🤖 AI Agent:**
> Fetching details for server 12345... It is a CX21 instance located in fsn1-dc14, currently running Ubuntu 22.04 with IP 1.2.3.4.

---

**👤 You:**
> "Power on the server with ID 12347."

**🤖 AI Agent:**
> Sending power-on command to server 12347... The action has been initiated successfully.


## ❓ FAQ

**Q: Can I see the status of all my cloud servers at once?**
Yes, the `list_servers` tool retrieves a complete list of your instances, including their IDs, status, and labels.

**Q: Is it possible to turn on a server that is currently powered off?**
Absolutely. Use the `poweron_server` tool with the specific Server ID to initiate the power-on sequence.

**Q: Can I manage security rules through this integration?**
Yes, you can use `list_firewalls` to audit existing rules and `create_firewall` to set up new protection layers for your infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hetzner](https://vinkius.com/mcp/hetzner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hetzner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hetzner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hetzner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hetzner": {
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
