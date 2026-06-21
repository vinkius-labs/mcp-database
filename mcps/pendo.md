# Pendo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pendo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pendo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pendo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage product engagement via Pendo — list guides, track page views, and analyze visitor behavior directly from any AI agent.

## Description
Connect your **Pendo** subscription to any AI agent and take full control of your product adoption and user engagement workflows through natural conversation.

### What you can do

- **Guide Management** — List all in-app guides and retrieve detailed metadata and performance metrics.
- **User & Account Insights** — Look up detailed profiles for visitors and accounts to understand their journey.
- **Product Tagging Auditing** — List defined pages and features to verify your product instrumentation.
- **Metadata Schema Discovery** — Retrieve schemas for visitor and account metadata to understand available data points.
- **Segment Overview** — List saved user segments to maintain visibility over your audience targeting.

### How it works

1. Subscribe to this server
2. Enter your Pendo Integration Key
3. Start optimizing your product experience from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check guide performance or verify if a feature is correctly tagged.
- **Customer Success Managers** — lookup visitor activity and account metadata during high-pressure support cases.
- **Growth Engineers** — audit segments and metadata schemas while implementing new tracking events.


## Available Tools
- **get_pendo_account**: Get details for a specific account
- **get_pendo_guide_metrics**: Get performance metrics for a guide
- **get_pendo_guide**: Get details for a specific guide
- **get_pendo_visitor**: Get details for a specific visitor
- **list_pendo_applications**: List applications tracked in the Pendo subscription
- **list_pendo_features**: List tagged features
- **list_pendo_guides**: ) defined in Pendo.

List Pendo guides
- **list_pendo_metadata_schema**: List metadata schema definitions
- **list_pendo_pages**: List tagged pages
- **list_pendo_segments**: List saved user segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pendo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active guides in my Pendo account."

**🤖 AI Agent:**
> I've retrieved 12 guides. Notable ones include 'New Feature Announcement', 'Onboarding Checklist', and 'Satisfaction Survey'. Which one would you like to see metrics for?

---

**👤 You:**
> "Get metadata for visitor 'user@example.com'."

**🤖 AI Agent:**
> Visitor 'user@example.com' is associated with account 'Global Corp'. Their properties include role: 'admin', trial_end: '2026-12-01', and they have viewed 45 pages in the last 30 days.

---

**👤 You:**
> "Show me the performance metrics for the guide 'guide_98765'."

**🤖 AI Agent:**
> Guide 'guide_98765' has been viewed by 1,250 unique visitors with a 68% click-through rate and 45% completion rate.


## Installation & Usage

To install and use the **Pendo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pendo](https://vinkius.com/mcp/pendo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
