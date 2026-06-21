# Beehiiv MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beehiiv)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/beehiiv-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/beehiiv-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Automate newsletter management via Beehiiv — manage publications, subscribers, analytics, and posts natively with your AI agent.

## Description
Connect your **Beehiiv** account to any AI agent and empower it to operate your entire newsletter growth engine, analyzing open rates, verifying automated sequences, and maintaining audience health directly from chat.

### What you can do

- **Subscribers & Audience** — Browse email lists, fetch UTM acquisition params, and explicitly register new subscribers with single commands
- **Post Metadata & Content** — Retrieve pure HTML payloads of delivered newsletters and paginate through full historical posts
- **Real-Time Analytics** — Generate comprehensive overviews of account-level performance, highlighting macroscopic open and click rates
- **Segments & Automations** — Explore active internal audience segments and conditional email logic chains dynamically
- **Publication Topology** — Investigate overriding active metrics linking directly to your organization's core structure

### How it works

1. Subscribe to this server
2. Enter your precise Beehiiv Publication ID and API Key
3. Start fetching and sending audience signals from Claude, Cursor, or any MCP-compatible environment

Eliminate the friction of switching tabs between IDEs and your ESP. Keep writing code while your AI orchestrates email interactions.

### Who is this for?

- **Growth Engineers** — script custom subscription pipelines and troubleshoot active programmatic endpoints on the fly
- **Content Creators & Writers** — pull open rate metrics or read historical post structures while drafting the next edition
- **Marketing Leads** — audit behavioral conditions and track segment isolation safely through quick questions


## Available Tools
- **list_publications**: List active Beehiiv publications
- **get_publication**: Get specific Beehiiv publication metadata
- **list_subscriptions**: List specific Beehiiv active subscribers
- **get_subscription**: Get exact details of a Beehiiv subscription
- **create_subscription**: Register a new subscriber explicitly
- **list_posts**: List explicit newsletter posts natively published
- **get_post**: Retrieve explicit content of a specific Post
- **get_post_stats**: Get aggregated post performance statistics
- **list_segments**: List specific internal Beehiiv segments
- **list_automations**: List native conditional email journeys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beehiiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent newsletter publications and ID formats."

**🤖 AI Agent:**
> I found 1 active publication linked: 'Tech Growth Daily' under ID 'pub_1234abcd-xxxx'. It's natively configured pointing to origin parameters tracking the domain effectively.

---

**👤 You:**
> "Check overall open and click stats for my account."

**🤖 AI Agent:**
> Here is the summary output tracking aggregate performance: Overall open rate stands at precisely 46.2%, converting active click ratios to 4.5% resolving across 8,400 active receivers derived directly from macro endpoints.

---

**👤 You:**
> "Subscribe alex@example.com to my newsletter right now."

**🤖 AI Agent:**
> Success! Explicit subscription request executed properly. The user alex@example.com has actively landed on the recipient pool correctly and will resolve in future workflows securely.


## Installation & Usage

To install and use the **Beehiiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beehiiv](https://vinkius.com/mcp/beehiiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
