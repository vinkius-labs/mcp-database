# Kavkom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kavkom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kavkom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kavkom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Set up a professional cloud phone system with call routing, IVR menus, and analytics designed for European businesses.

## Description
Connect your **Kavkom** account to any AI agent and manage phone communications through natural conversation.

### What you can do

- **Contact Management** — List and inspect contacts with call history
- **Call Logs** — Browse call history with duration, direction, and status
- **Phone Lines** — List available phone lines and their assignments
- **Voicemail** — Access voicemail messages with transcripts
- **Call Recordings** — Retrieve and review call recordings

### How it works

1. Subscribe to this server
2. Enter your Kavkom API Token
3. Start managing calls from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — track call activity and manage contacts
- **Support Teams** — review call logs and voicemails
- **Managers** — monitor team phone usage and performance


## Available Tools
- **create_contact**: Add a new contact
- **get_call_details**: Get details for a specific call
- **list_calls**: List Kavkom call history
- **list_crm_contacts**: List synced contacts
- **list_sms_history**: List sent and received SMS
- **list_team_members**: List account users
- **send_sms_message**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kavkom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show today's call log and any pending voicemails."

**🤖 AI Agent:**
> Today: 22 calls. Inbound: 14 (avg 3.8 min). Outbound: 8 (avg 5.2 min). Missed: 3. Voicemails: 2 pending. 1) +33-1-4567-8901 (2 min, 10:30 AM): 'Calling about the proposal...' 2) +33-6-1234-5678 (1 min, 11:15 AM): 'Please call back regarding invoice.'

---

**👤 You:**
> "List all contacts and the phone lines assigned to the team."

**🤖 AI Agent:**
> Contacts: 156. Recent: Ana Costa (12 calls), James Lee (8 calls), Lisa Park (5 calls). Phone lines: 5 active. +33-1-4567-0001 (Main, Sarah). +33-1-4567-0002 (Support, Mike). +33-1-4567-0003 (Sales, Lisa). 2 unassigned.

---

**👤 You:**
> "Show call recordings from this week for the sales line."

**🤖 AI Agent:**
> Sales line (+33-1-4567-0003): 18 calls this week. Recordings: 15 available. Longest: 'Enterprise Deal' (22 min, Lisa). Total recording time: 3h 45m. Top contacts called: Acme Corp (5 calls), TechCo (3 calls).


## Installation & Usage

To install and use the **Kavkom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kavkom](https://vinkius.com/mcp/kavkom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
