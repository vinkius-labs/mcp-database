# World Time (Keyless) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-time-keyless)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/world-time-keyless-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/world-time-keyless-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Get precise current atomic time, UTC offsets, and DST states for any timezone worldwide — no API key required.

## Description
Connect to the **World Time API** and empower your AI agent with precise, synchronized time data through natural conversation. This server provides micro-service level access to atomic time across all IANA timezone regions without requiring any manual signups or complex API keys.

### What you can do

- **Precise Synchronization** — Retrieve the exact current time for any valid IANA region (e.g., 'Europe/London' or 'America/New_York') with millisecond precision
- **Offset Discovery** — Verify the current UTC offset and check whether a specific location is currently observing Daylight Saving Time (DST)
- **Timezone Browsing** — List all supported timezone strings to ensure you are using the correct identifier for your requests
- **IP-Based Inference** — Automatically retrieve the current local time based on the inferred location of the network IP address
- **Standardized Data** — Access high-quality JSON responses including Unix timestamps, day of year, and week number for scheduling purposes
- **Global Coverage** — Get reliable time data for any part of the world, from major cities to remote islands

### How it works

1. Subscribe to this server
2. No API Key required (just click connect)
3. Start asking about the time in any city through Claude, Cursor, or any MCP-compatible client

No more manual math to figure out a time difference. Your AI agent becomes your global master clock.

### Who is this for?

- **Developers** — verify UTC offsets and time synchronization for server-side logging or scheduling
- **Project Managers** — quickly check local times for distributed team members before planning meetings
- **Operations Teams** — monitor DST transitions and verify week numbers for business reporting
- **Everyday Users** — find out what time it is anywhere in the world through a simple chat command


## Available Tools
- **get_current_time**: You can provide a timezone string (e.g. "America/Sao_Paulo") or use "ip" to infer from the network.

Retrieves the exact current atomic time, UTC offset, and DST state for a specified timezone
- **list_available_timezones**: Lists all valid timezone regions (e.g. Europe/London) supported by the World Time API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Time (Keyless)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What time is it in Tokyo right now?"

**🤖 AI Agent:**
> In Tokyo (Asia/Tokyo), it is currently Tuesday, March 31, 2026, at 09:15 PM. The UTC offset is +09:00 and they are not currently observing Daylight Saving Time.

---

**👤 You:**
> "Check the current time based on my IP."

**🤖 AI Agent:**
> Based on your network IP, your local time is 10:30 AM. Your timezone is America/Sao_Paulo (UTC -03:00).

---

**👤 You:**
> "Is London currently in Daylight Saving Time?"

**🤖 AI Agent:**
> Checking Europe/London… Yes, London is currently observing Daylight Saving Time (BST). The offset is UTC +01:00. The transition back to GMT will occur later this year.


## Installation & Usage

To install and use the **World Time (Keyless)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-time-keyless](https://vinkius.com/mcp/world-time-keyless)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
