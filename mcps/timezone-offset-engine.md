# Timezone Offset Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timezone-offset-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/timezone-offset-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/timezone-offset-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the exact offset between two timezones at any moment, with full DST awareness. Powered by Luxon.

## Description
When a scheduling agent needs to know the time difference between São Paulo and London on July 15th, the answer changes depending on DST. LLMs get DST wrong 100% of the time. This MCP uses Luxon with the full IANA timezone database.

### The Superpowers

- **DST Aware:** Calculates offsets at a specific moment, correctly handling all DST transitions worldwide.
- **Full IANA Database:** Supports all 400+ IANA timezones (America/Sao_Paulo, Europe/London, Asia/Kolkata, etc.).
- **Bidirectional:** Shows both the source and target local times plus the exact offset in hours and minutes.


## Available Tools
- **get_timezone_offset**: Pass two IANA timezone names (e.g. "America/Sao_Paulo", "Europe/London") and optionally an ISO 8601 datetime. The engine returns the exact offset in hours/minutes and whether each zone is in DST. Never calculate DST offsets yourself — you will get it wrong.

Calculates the exact offset between two IANA timezones at a specific moment, respecting Daylight Saving Time (DST). Powered by Luxon


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timezone Offset Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the time difference between São Paulo and London on July 15, 2025?"

**🤖 AI Agent:**
> Offset: +4 hours (London is in BST/DST, São Paulo is not).

---

**👤 You:**
> "If it's 9am in Tokyo right now, what time is it in New York?"

**🤖 AI Agent:**
> Tokyo 09:00 JST → New York 20:00 EDT (-13 hours).

---

**👤 You:**
> "Will the offset between Berlin and Sydney change in March 2025?"

**🤖 AI Agent:**
> Yes. Check March 1 vs March 31 — DST transitions in both hemispheres change the offset.


## Installation & Usage

To install and use the **Timezone Offset Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timezone-offset-engine](https://vinkius.com/mcp/timezone-offset-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
