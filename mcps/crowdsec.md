# CrowdSec MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdsec)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crowdsec-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crowdsec-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate threat intelligence via CrowdSec — query local decisions, stream security updates, and check global IP reputation directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrowdSec** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if there are any active decisions for IP 1.2.3.4 in our local CrowdSec database."

**🤖 AI Agent:**
> I've checked the Local API. There is one active decision for 1.2.3.4: a 'ban' applied 2 hours ago due to 'http-backdoor-attempts'. It is set to expire in 22 hours.

---

**👤 You:**
> "Get the latest stream of decisions from CrowdSec to see recent blocks."

**🤖 AI Agent:**
> Polling the decision stream... I found 3 new bans in the last few minutes involving IPs from the 193.x.x.x range targeting SSH services. No decisions were deleted in this interval.

---

**👤 You:**
> "What is the global reputation of IP 185.220.101.101 according to CrowdSec CTI?"

**🤖 AI Agent:**
> According to CrowdSec CTI, 185.220.101.101 is classified as a 'Tor Exit Node'. It has a high noise score and is frequently reported for scanning activities globally. It is currently flagged in multiple community blocklists.


## Installation & Usage

To install and use the **CrowdSec** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdsec](https://vinkius.com/mcp/crowdsec)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
