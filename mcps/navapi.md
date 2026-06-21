# NavAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/navapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/navapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/navapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage maritime navigation — audit ports, routes, and traffic via AI.

## Description
Empower your AI agent to orchestrate your entire maritime research and nautical auditing workflow with **NavAPI**, the comprehensive source for global shipping and navigation data. By connecting NavAPI to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for maritime ports, audit nautical distances, and retrieve vessel traffic statistics without you ever touching a technical portal. Whether you are planning shipping routes or conducting regional maritime audits, your agent acts as a real-time nautical consultant, ensuring your data is always precise and localized.

### What you can do

- **Port Auditing** — Retrieve high-resolution details for thousands of global maritime ports, including country and coordinate metadata.
- **Route Oversight** — Audit nautical distances between any two ports to maintain a clear view of shipping logistics and scale.
- **Traffic Intelligence** — Query real-time vessel traffic for specific ports to understand the current industry distribution instantly.
- **Chart Discovery** — List available nautical charts for specific geographic areas to assist in regional navigation planning.
- **Logistics Monitoring** — Check API status to ensure your maritime research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your NavAPI.com API Key
3. Start managing your maritime intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Analysts** — monitor port traffic and retrieve nautical metadata straight from your workflow.
- **Trade Researchers** — verify shipping routes and audit regional distribution without manual searching.
- **Ship Operators** — perform rapid audits of port distances and identify relevant charts through natural language.
- **Operations Leads** — automate nautical data querying to orchestrate cross-functional logistics teams smoothly.


## Available Tools
- **check_api_status**: Check if the NavAPI service is operational
- **get_port_distance**: Calculate the nautical distance between two ports
- **get_nautical_ports**: List global maritime ports with optional country filter
- **get_port_vessel_traffic**: Get current vessel traffic statistics for a specific port
- **list_nautical_charts**: List nautical charts available for a specific geographic area
- **search_maritime_routes**: Search for maritime shipping routes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NavAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for ports in 'Singapore' using NavAPI."

**🤖 AI Agent:**
> I've retrieved the ports for Singapore! The primary entry is the Port of Singapore (ID: SGSIN). Would you like to see the current vessel traffic or the available nautical charts for this region?

---

**👤 You:**
> "Calculate the nautical distance between 'SGSIN' (Singapore) and 'NLRTM' (Rotterdam)."

**🤖 AI Agent:**
> The nautical distance between Singapore and Rotterdam is approximately 8,300 NM via the Suez Canal. I can assist you with more route auditing if needed.

---

**👤 You:**
> "What is the current traffic at the Port of Shanghai (CNSHA)?"

**🤖 AI Agent:**
> I've retrieved the real-time traffic for Shanghai! There are currently over 200 vessels identified in the port area. Notable categories include container ships and bulk carriers. I can provide the breakdown by vessel type if you'd like.


## Installation & Usage

To install and use the **NavAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/navapi](https://vinkius.com/mcp/navapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
