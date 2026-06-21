# IP Parking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ip-parking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ip-parking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ip-parking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage PARCS operations: sites, tariffs, gates, and ANPR events via IP Parking API.

## Description
Connect **IP Parking** to any AI agent and streamline your Parking Access and Revenue Control System (PARCS) — manage occupancy, update tariffs, control gates, and audit transactions through natural conversation.

### What you can do
- **Site Management** — Monitor real-time occupancy and revenue across all locations
- **Tariff Configuration** — View and modify hourly rates and pricing rules instantly
- **Gate Control** — Remotely open/close barriers for assistance or maintenance
- **Hardware Monitoring** — Check health of ANPR cameras, ticket dispensers, and gates
- **Transaction Auditing** — Review exit logs and revenue collection
- **ANPR Integration** — Register or simulate license plate recognition events

### How it works
1. Subscribe to this server
2. Enter your IP Parking API Key and Base URL
3. Start managing your parking infrastructure from Claude, Cursor, or any MCP-compatible client

IP Parking is a Dutch developer of web-based PARCS hardware and software, enabling barrierless and smart parking solutions.

### Who is this for?
- **Parking Operators** — Adjust tariffs and check occupancy without logging into the central management system
- **Support Teams** — Remotely open stuck gates and verify camera status via voice or text commands
- **Revenue Auditors** — Quickly query transaction logs and verify daily income


## Available Tools
- **register_anpr**: Used for testing or manual override of entry/exit.

Simulate or register an ANPR (License Plate Recognition) event
- **control_gate**: Remotely open or close a barrier gate.. Actions: default
- **list_hardware**: List hardware status (ANPR cameras, ticket machines, gates)
- **get_site_status**: Get real-time occupancy and revenue status for a site
- **list_sites**: List all managed parking sites
- **get_system_health**: Get overall system health and connectivity status
- **list_tariffs**: List active tariff rules
- **get_ticket_details**: Get details of a specific parking ticket/session
- **list_transactions**: List recent exit transactions and revenue logs
- **update_tariff**: Use this to adjust hourly rates or caps.

Update tariff rules or rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IP Parking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the occupancy of Site A."

**🤖 AI Agent:**
> Site A: 142 available spaces out of 200 (71% full). Today's revenue: €1,250.

---

**👤 You:**
> "Open gate 3 for a manual exit."

**🤖 AI Agent:**
> Gate 3 command sent: 'open'. Barrier is now open. Ticket cycle reset.

---

**👤 You:**
> "Update tariff 'Standard' to €4.50 per hour."

**🤖 AI Agent:**
> Tariff 'Standard' updated successfully. New rate: €4.50/hr. All ticket machines synchronized.


## Installation & Usage

To install and use the **IP Parking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ip-parking](https://vinkius.com/mcp/ip-parking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
