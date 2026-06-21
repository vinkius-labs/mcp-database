# Segment MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/segment)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/segment-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/segment-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent with read access to your Segment workspace to audit sources, destinations, warehouses, and tracking plans natively.

## Description
Connect your **Twilio Segment** CDP to any AI agent to interact with your customer data infrastructure conversationally. Give your agent the ability to map data pipelines and verify tracking schemas exactly as they reflect in production without leaving the chat interface.

### What you can do

- **Map Pipelines** — Instruct your AI to list all active Sources (Web, iOS, Android) and immediately see which Destinations they route data to
- **Audit Tracking Plans** — Pull in specific event tracking schemas or 'Tracking Plans' to confirm payload structures with developers effortlessly
- **Review Warehousing** — Have the agent list all authorized Data Warehouses hooked into the workspace to confirm downstream compliance
- **Governance Automation** — Query unique namespace IDs directly from the Public API without needing to click through slow dashboard settings

### How it works

1. Subscribe to this integration
2. Provide a 'Public API Token' from your Segment admin panel
3. Start commanding your agent to audit your routing ecosystem from Claude, Cursor, or your preferred MCP terminal

### Who is this for?

- **Data Engineers** — ask the AI to retrieve the detailed tracking plan event schemas so you can write exact tracking code in your frontend repository
- **RevOps & Growth** — ask the AI to map which destinations are connected to your main SaaS app source to ensure no tool is left behind
- **Analytics Teams** — quickly check the raw source IDs to properly configure a new BI dashboard parameter


## Available Tools
- **get_source**: Retrieves details for a specific data source
- **get_tracking_plan**: Retrieves details for a specific tracking plan
- **get_workspace**: Retrieves information about the current Segment workspace
- **list_destinations**: Lists all destinations configured for a specific source
- **list_sources**: Lists all data sources in the Segment workspace
- **list_tracking_plans**: Lists all tracking plans in the workspace
- **list_warehouses**: Lists all data warehouses configured in the workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Segment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Workspaces configured in the environment."

**🤖 AI Agent:**
> I've queried the workspace configurations. Your primary environment is currently named 'Global Operations (vinkius_corp)' containing 12 active sources and maintaining a stable 30-day API limit threshold.

---

**👤 You:**
> "Lookup the Tracking Plan mapped to ID 'tp_123' to see the exact structure required for the Checkout Started event."

**🤖 AI Agent:**
> The Tracking Plan requires the 'Checkout Started' event to pass an array of product mappings. Essential properties include: `cart_id` (string), `total_value` (float), and `currency` (string, ISO 4217). Knowing this, I can draft the necessary React context hook for you.

---

**👤 You:**
> "Identify all data Warehouses we have feeding from this Segment workspace."

**🤖 AI Agent:**
> I've located 2 active warehouses attached to this workspace. First is a Snowflake cluster stationed securely behind VPC ('snowflake_eu_prod'). Second is an Amazon Redshift instance ('redshift_analytic_db'). Both register with healthy ping statuses according to Segment.


## Installation & Usage

To install and use the **Segment** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/segment](https://vinkius.com/mcp/segment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
