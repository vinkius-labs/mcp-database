# Salespanel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salespanel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/salespanel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/salespanel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate lead tracking and visitor intelligence via Salespanel — manage contacts, website visitors, and engagement directly from any AI agent.

## Description
Connect your **Salespanel** account to any AI agent and simplify your lead tracking, visitor intelligence, and marketing automation through natural conversation.

### What you can do

- **Contact Management** — List all identified contacts and leads, retrieve detailed metadata, and monitor lead scores and status
- **Visitor Intelligence** — Access a list of recent anonymous and identified website visitors to understand your traffic
- **Engagement tracking** — Query tracking events and user actions to stay on top of your customer journey
- **Activity Feeds** — Monitor real-time activity feeds to see who is interacting with your content right now
- **Segment Control** — Query lead segments to choose the right context for each outreach and qualification step

### How it works

1. Subscribe to this server
2. Enter your Salespanel API Token from your account settings
3. Start managing your lead intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_company**: Get details for a specific company
- **get_segment**: Get details for a specific segment
- **get_visitor**: Get details for a specific website visitor
- **list_accounts**: List all tracked accounts
- **list_companies**: List all identified companies
- **get_contact_details**: Get details for a specific contact
- **list_contacts**: List Salespanel contacts
- **list_engagement_events**: List tracking events
- **list_activity_feeds**: List activity feeds
- **list_lead_segments**: List lead segments
- **list_anonymous_visitors**: List recent website visitors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salespanel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all identified contacts in Salespanel."

**🤖 AI Agent:**
> I've retrieved your identified contacts. You have 50 identified leads, including 'John Doe' (Lead Score: 85) and 'Jane Smith'.

---

**👤 You:**
> "Show me the top website visitors from this week with their lead scores and company identification."

**🤖 AI Agent:**
> Top 10 website visitors this week by engagement. #1: David Chen (Meridian Corp, 340 employees). Lead score: 94. Pages viewed: 23 (pricing: 4 visits, case studies: 3, API docs: 5). Time on site: 47 minutes across 6 sessions. #2: Sarah Kim (DataForge, 120 employees). Score: 87. Pages: 18 (product tour: 3 visits). #3: Anonymous visitor from TechVentures IP range. Score: 78. Total identified visitors: 234. Companies identified: 89. Hot leads (score >80): 12. Conversion events: 8 demo requests, 5 whitepaper downloads.

---

**👤 You:**
> "Show me the visitor journey and all touchpoints for the Meridian Corp lead."

**🤖 AI Agent:**
> Meridian Corp lead journey (David Chen). Day 1: First visit via Google search "enterprise API platform". Viewed homepage and features page (3 min). Day 3: Returned directly. Read 2 case studies and pricing page (12 min). Day 5: Downloaded whitepaper "API-First Architecture Guide" (form submitted). Day 7: Attended webinar "Scaling Enterprise APIs". Day 9: 3 visits to API documentation (22 min total). Day 10: Visited pricing page twice, opened comparison page. Day 11 (today): Submitted demo request form. Total touchpoints: 14. Lead score trajectory: 25 → 94.


## Installation & Usage

To install and use the **Salespanel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salespanel](https://vinkius.com/mcp/salespanel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
