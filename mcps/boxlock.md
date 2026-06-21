# BoxLock MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boxlock)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boxlock-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boxlock-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Secure package deliveries with smart lockbox technology that verifies carriers and prevents porch theft at the door.

## Description
Connect your **BoxLock Control** (v3) account to any AI agent and take full control of your physical security and automated supply chain logistics through natural conversation.

### What you can do

- **Lock Orchestration** — List and manage all BoxLock smart locks in your organization programmatically, retrieving detailed battery levels and high-fidelity connectivity status
- **Remote Authorization** — Programmatically authorize locks to be opened via physical button press for specific workers or maintenance windows in real-time
- **Access Intelligence** — Monitor real-time access events and retrieve detailed historical activity logs to maintain high-fidelity audit trails of all openings and scans
- **Asset Tracking Architecture** — Access complete directories of barcodes and trackable assets to maintain a perfectly coordinated digital ledger of physical goods
- **Location Visibility** — Retrieve complete directories of physical sites and groups to coordinate your infrastructure security directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Bearer Token) from your BoxLock Control dashboard (Settings > Developer API)
3. Start managing your physical access from Claude, Cursor, or any MCP client

No more manual status checking of individual locks or missing delivery attempts. Your AI acts as your dedicated security operations and logistics coordinator.

### Who is this for?

- **Logistics Managers** — instantly authorize delivery access and monitor asset scans using natural language commands
- **Facility Operations** — track lock battery health and manage worker permissions without leaving your workspace
- **Security Teams** — automate the auditing of physical access events and monitor tampering alerts through simple AI queries


## Available Tools
- **get_lock**: Get lock details
- **list_activities**: List lock activity logs
- **list_barcodes**: List all active barcodes
- **list_locations**: List all locations
- **list_locks**: List all BoxLock smart locks
- **list_users**: List all organization users
- **press_to_open**: Pass data as a JSON string.

Remotely authorize a lock to be opened


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoxLock** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active smart locks in my organization."

**🤖 AI Agent:**
> I've retrieved your smart locks. You currently have 5 active devices, including 'Front Gate' (Battery: 85%) and 'Loading Dock B'. Which one would you like to inspect for activity logs?

---

**👤 You:**
> "Authorize 'Loading Dock B' (ID: 'lock_123') to be opened for worker '101' for the next hour."

**🤖 AI Agent:**
> Remote opening authorized! The lock 'Loading Dock B' can now be opened when the physical button is pressed by worker 101. The authorization expires in 60 minutes. Shall I monitor for the opening event?

---

**👤 You:**
> "Show the last 5 access events for all locks from today."

**🤖 AI Agent:**
> Accessing audit logs... Today's last 5 events include 3 successful openings at 'Warehouse West' and 2 barcode scans for asset 'P-500'. All interactions were within high-fidelity norms. Need more historical context?


## Installation & Usage

To install and use the **BoxLock** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boxlock](https://vinkius.com/mcp/boxlock)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
