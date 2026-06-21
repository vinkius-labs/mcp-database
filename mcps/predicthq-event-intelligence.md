# PredictHQ Event Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/predicthq-event-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/predicthq-event-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/predicthq-event-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage global events — audit festivals, sports, and rankings via AI.

## Description
Empower your AI agent to orchestrate your entire event research and demand auditing workflow with **PredictHQ**, the authoritative source for intelligent event data. By connecting PredictHQ to your agent, you transform complex event searches into a natural conversation. Your agent can instantly search for global festivals, sports matches, and conferences, audit attendance rankings, and query specific location metadata without you ever touching an event portal. Whether you are conducting market demand research or managing regional operational constraints, your agent acts as a real-time event consultant, ensuring your data is always verified and precise.

### What you can do

- **Event Auditing** — Search for thousands of global events by keyword or category and retrieve detailed metadata, including start times and rankings.
- **Ranking Oversight** — Audit the PredictHQ impact rank for specific events to understand the current industry lead in attendance scale instantly.
- **Category Discovery** — Browse available event categories like 'concerts', 'sports', or 'festivals' to identify relevant thematic markers for your audience.
- **Geographic Intelligence** — Retrieve high-resolution location metadata for specific event IDs to assist in deep-dive logistics classification.
- **Operational Monitoring** — Check API status to ensure your event research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your PredictHQ API Key
3. Start managing your event intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Demand Analysts & Marketers** — monitor event trends and retrieve official impact metadata straight from your workflow.
- **Logistics Managers** — verify event locations and audit attendance patterns without manual searching.
- **Business Planners** — perform rapid audits of local events and identify relevant demand markers through natural language.
- **Operations Leads** — automate event data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **check_api_status**: Check if the PredictHQ service is operational
- **get_event_details**: Get full metadata and ranking for a specific event ID
- **list_event_categories**: List common event categories supported by PredictHQ
- **search_predict_events**: Search for global events (concerts, sports, festivals) using PredictHQ


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PredictHQ Event Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for concerts in 'London' for next month using PredictHQ."

**🤖 AI Agent:**
> I've retrieved several concerts in London! Notable entries include [Artist] at the O2 Arena. I can provide the PredictHQ rank and start time metadata for each of these events if you'd like.

---

**👤 You:**
> "What is the impact ranking for event ID '12345'?"

**🤖 AI Agent:**
> I've retrieved the details for event 12345! It has a PHQ Rank of 85, identified as a 'Major' event with high attendance expectations. I can assist you with the location and category metadata for this site.

---

**👤 You:**
> "List event categories supported by PredictHQ."

**🤖 AI Agent:**
> I've retrieved the category catalog! Notable groups include 'concerts', 'sports', 'festivals', and 'conferences'. I can help you search for specific events in any of these thematic clusters.


## Installation & Usage

To install and use the **PredictHQ Event Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/predicthq-event-intelligence](https://vinkius.com/mcp/predicthq-event-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
