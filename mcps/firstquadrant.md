# FirstQuadrant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firstquadrant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firstquadrant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firstquadrant-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Let AI handle your outbound sales prospecting with autonomous research, personalized messaging, and smart follow-up sequences.

## Description
Connect your **FirstQuadrant** account to any AI agent and take full control of your B2B sales pipeline and contact enrichment workflows through natural conversation.

### What you can do

- **Lead Orchestration** — List and manage your complete database of leads and contacts, including retrieving detailed metadata and performing search lookups programmatically
- **AI Enrichment** — Trigger autonomous AI workflows to gather deep context about a lead from external sources and update contact profiles automatically
- **Campaign Management** — Access available sales sequences and enroll contacts into personalized email campaigns directly through your agent
- **Schema Intelligence** — Explore and manage your custom property schema to ensure all sales data is perfectly structured for AI analysis
- **Activity Monitoring** — Monitor the complete log of sales activities, including emails, calls, and AI-driven tasks in real-time

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Organization ID** from FirstQuadrant (Settings > Developer Settings)
3. Start managing your B2B sales pipeline from Claude, Cursor, or any MCP client

No more manual contact research or complex campaign toggling. Your AI acts as your dedicated sales operations coordinator.

### Who is this for?

- **Sales Development Reps (SDRs)** — instantly identify top leads and trigger enrichment workflows using natural language
- **Account Managers** — retrieve full interaction histories and verify contact details without leaving your workspace
- **Growth Teams** — automate lead discovery and scale personalized outreach through simple AI queries


## Available Tools
- **add_to_campaign**: Add contact to a campaign
- **create_contact**: Create a new lead/contact
- **enrich_contact_ai**: Trigger AI enrichment for a contact
- **get_contact_details**: Get contact profile details
- **list_activities**: List sales activities
- **list_campaigns**: List sales campaigns/sequences
- **list_contacts**: Supports advanced filtering by email or created date.

List FirstQuadrant contacts
- **list_properties_schema**: List custom properties schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FirstQuadrant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all qualified leads from FirstQuadrant."

**🤖 AI Agent:**
> I've retrieved your leads. You have 12 qualified contacts, including 'John Doe' (ID: 101) and 'Sarah Smith' (ID: 102). Would you like to see the interaction history for any of them?

---

**👤 You:**
> "Enrich the contact with email 'ceo@acme.com'."

**🤖 AI Agent:**
> AI enrichment triggered! I've started the research workflow for ceo@acme.com. I'll notify you as soon as the company size and latest funding details are added to the profile.

---

**👤 You:**
> "Add contact '101' to the 'Discovery Sequence'."

**🤖 AI Agent:**
> Contact enrolled! I've successfully added John Doe (ID: 101) to your 'Discovery Sequence'. They will receive the first automated email shortly.


## Installation & Usage

To install and use the **FirstQuadrant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firstquadrant](https://vinkius.com/mcp/firstquadrant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
