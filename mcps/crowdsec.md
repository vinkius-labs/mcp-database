# CrowdSec MCP Server

Automate threat intelligence via CrowdSec — query local decisions, stream security updates, and check global IP reputation directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdsec)

## Overview
**Category:** fort-knox
**Tools Count:** 3

## Description
Connect your **CrowdSec** security engine to any AI agent to take full control of your threat intelligence and network defense through natural conversation.

### What you can do

- **Local Decisions** — Query your Local API (LAPI) for active blocks or decisions on specific IPs, ranges, or scopes to understand current local threats.
- **Decision Streaming** — Poll for real-time updates on new and deleted decisions from your local database to keep your security context synchronized.
- **Global CTI Reputation** — Fetch global IP reputation data, behaviors, and classifications from the CrowdSec Community Threat Intelligence (CTI) network.
- **Security Auditing** — Inspect metadata and classifications for suspicious actors directly from your command interface or code editor.

### How it works

1. Subscribe to this server
2. Enter your CrowdSec LAPI URL, LAPI Key, and CTI Key
3. Start managing your security posture from Claude, Cursor, or any MCP-compatible client

No more manual log diving or complex CLI commands to check if an IP is malicious. Your AI acts as a dedicated security analyst.

### Who is this for?

- **Security Engineers** — instantly retrieve local decision statuses and global reputation metrics without leaving the terminal
- **DevOps Teams** — monitor security streams and verify IP behaviors during incident response directly from the IDE
- **System Administrators** — automate the auditing of blocked ranges and suspicious network activity through natural language


## Available Tools
- **get_cti_smoke**: Get CTI reputation for an IP
- **get_decisions_stream**: Poll for new and deleted decisions from LAPI
- **get_decisions**: Query CrowdSec LAPI for decisions


## Installation & Usage

To install and use the **CrowdSec** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdsec](https://vinkius.com/mcp/crowdsec)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
