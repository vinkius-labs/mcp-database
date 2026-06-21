# SafeCube Container Tracking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/safecube-container-tracking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/safecube-container-tracking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/safecube-container-tracking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track maritime containers — audit shipments and events via AI.

## Description
Empower your AI agent to orchestrate your entire maritime logistics and container auditing workflow with **SafeCube**, the comprehensive source for real-time shipment data. By connecting the SafeCube API to your agent, you transform complex tracking searches into a natural conversation. Your agent can instantly retrieve container positions, audit active shipment statuses, and query historical tracking events without you ever touching a logistics dashboard. Whether you are managing supply chain visibility or monitoring regional port delays, your agent acts as a real-time maritime consultant, ensuring your data is always precise and up-to-the-minute.

### What you can do

- **Container Auditing** — Retrieve high-resolution tracking details for any maritime container by number, including status and vessel metadata.
- **Shipment Oversight** — Audit all active shipments in your account to maintain a clear view of global logistics and scale.
- **Event Discovery** — Retrieve detailed tracking events for specific shipment IDs to understand the temporal distribution of logistics milestones instantly.
- **Logistics Intelligence** — Query real-time ETA and position markers to assist in deep-dive supply chain classification.
- **Operational Monitoring** — Check API status to ensure your maritime tracking workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your SafeCube API Key
3. Start managing your maritime intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Supply Chain Analysts** — monitor container movements and retrieve official metadata straight from your workflow.
- **Logistics Managers** — verify shipment statuses and audit delivery patterns without manual searching.
- **Trade Researchers** — perform rapid audits of port arrivals and identify relevant logistics markers through natural language.
- **Operations Leads** — automate maritime data querying to orchestrate cross-functional shipping teams smoothly.


## Available Tools
- **check_api_status**: Check if the SafeCube service is operational
- **get_shipment_events**: Get a list of tracking events for a specific shipment ID
- **get_container_tracking**: Get real-time tracking data for a specific maritime container
- **list_active_shipments**: List all active shipments currently tracked in your SafeCube account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SafeCube Container Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track container 'TCNU1234567' using SafeCube."

**🤖 AI Agent:**
> I've retrieved the tracking data for container TCNU1234567! It is currently identified as 'En Route' aboard the vessel 'MSC OSCAR'. The current ETA is May 15th. Would you like the full event history metadata for this shipment?

---

**👤 You:**
> "List all my active shipments."

**🤖 AI Agent:**
> I've retrieved your active shipment catalog from SafeCube! You have 5 active containers, including 3 en route and 2 awaiting discharge. I can provide the unique shipment IDs and vessel metadata for each of these tracking records.

---

**👤 You:**
> "What are the latest events for shipment ID 'SHIP-123'?"

**🤖 AI Agent:**
> I've identified the events for shipment SHIP-123! The latest marker is 'Vessel Departure' from Singapore, recorded on May 10th. I can assist you with an audit of the previous port calls and duration markers if you'd like.


## Installation & Usage

To install and use the **SafeCube Container Tracking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safecube-container-tracking](https://vinkius.com/mcp/safecube-container-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
