# Appcues MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appcues-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/appcues-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/appcues-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Guide users through your product with in-app onboarding flows, feature announcements, and usage analytics without code.

## Description
Connect your **Appcues** account to any AI agent and take full control of your in-app onboarding and automated user experience orchestration through natural conversation.

### What you can do

- **Experience Portfolio Orchestration** — List and manage your entire portfolio of flows and checklists programmatically, retrieving detailed engagement metadata
- **User & Event Intelligence** — Programmatically monitor real-time user events and access behavioral metadata to coordinate your engagement strategy
- **Segment & Targeting Architecture** — Access your complete directory of user segments to coordinate your organizational resource allocation
- **Performance Monitoring** — Access real-time status updates for active flows and track individual completion metrics directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor event ingestion volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **API Secret** from your Appcues dashboard (Settings > API)
3. Start orchestrating your user growth from Claude, Cursor, or any MCP client

No more manual checking of individual flow completion rates or missing critical onboarding drop-offs. Your AI acts as your dedicated experience coordinator and user architect.

### Who is this for?

- **Product Managers** — instantly retrieve experience performance recaps and monitor onboarding health using natural language commands
- **Growth Leads** — verify individual user metadata and track event history without leaving your creative workspace
- **Developers** — integrate high-speed Appcues engagement data into custom analytics and CRM tools through simple AI queries


## Available Tools
- **check_appcues_status**: Verify Appcues API connectivity
- **delete_user**: This action is irreversible.

Delete a user from Appcues
- **get_flow**: Get flow details
- **get_segment**: Get segment details
- **get_user**: Get user profile from Appcues
- **list_checklists**: List all checklists
- **list_flows**: List all onboarding flows
- **list_segments**: List all user segments
- **publish_flow**: The flow must be in draft or unpublished state.

Publish a flow
- **unpublish_flow**: Users will no longer see it until republished.

Unpublish a flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appcues** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active flows in my Appcues account."

**🤖 AI Agent:**
> I've retrieved your experiences. You currently have 10 active flows, including 'New User Onboarding' and 'Feature Highlight B'. Would you like the detailed engagement metadata for any of them?

---

**👤 You:**
> "Show the completion rate for the 'Welcome Flow' from this week."

**🤖 AI Agent:**
> Experience intelligence orchestrated! For Welcome Flow, I've identified a completion rate of 70% from this week's users. I've retrieved the technical drop-off metadata for your review. Need help identifying where users are getting stuck?

---

**👤 You:**
> "Check for any active segments with zero engaged users this month."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 2 segments with zero engagement this month, including 'Trial Expired' and 'Inactive Beta'. I've retrieved the technical targeting metadata for your review. Shall I check for any pending experience updates for these groups?


## Installation & Usage

To install and use the **Appcues** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appcues-alternative](https://vinkius.com/mcp/appcues-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
