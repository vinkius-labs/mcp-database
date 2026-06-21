# Tuya MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tuya)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tuya-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tuya-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Control and monitor your Tuya IoT ecosystem — query device status and send real-time commands to smart hardware via AI.

## Description
Connect your **Tuya IoT** account to any AI agent and manage your smart home or industrial hardware through natural conversation.

### What you can do

- **Device Inspection** — Retrieve detailed metadata for any connected device, including its online status, category, and local key for advanced integrations.
- **Real-time Control** — Send precise commands to your hardware using standard instruction sets (e.g., toggling switches, adjusting brightness, or setting modes).
- **Status Monitoring** — Instantly check if your devices are reachable and functioning correctly within your cloud project.

### How it works

1. Subscribe to this server
2. Enter your Tuya Client ID, Secret, and Endpoint
3. Start controlling your smart environment from Claude, Cursor, or any MCP-compatible client

No more jumping between mobile apps to check if a sensor is online or to toggle a smart plug. Your AI acts as a centralized IoT dashboard.

### Who is this for?

- **Smart Home Enthusiasts** — manage complex automation setups and check device health directly from your workspace.
- **IoT Developers** — quickly inspect device categories and local keys while building or debugging integrations.
- **Facility Managers** — monitor and control distributed hardware across different locations using simple text commands.


## Available Tools
- **get_device**: Query Tuya device details
- **send_commands**: g., switch_led: true).

Send control commands to a Tuya device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tuya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status and details of device ID 'bf78234567890abcdef'."

**🤖 AI Agent:**
> I've queried the device. It is currently Online. It's a 'Smart Plug' (Category: cz) with the local key 'a1b2c3d4...'. Would you like to send any commands to it?

---

**👤 You:**
> "Turn on the LED for device 'eb4567890123456789'."

**🤖 AI Agent:**
> Command sent successfully. I've instructed device 'eb4567890123456789' to set 'switch_led' to true. The device has confirmed receipt of the command.

---

**👤 You:**
> "Is my smart heater (ID: 0123456789) reachable right now?"

**🤖 AI Agent:**
> Checking connectivity... Yes, the smart heater is currently reporting as Online in the Tuya Cloud. Its last heartbeat was received successfully.


## Installation & Usage

To install and use the **Tuya** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tuya](https://vinkius.com/mcp/tuya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
