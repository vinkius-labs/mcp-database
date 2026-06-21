# Refiner MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/refiner)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/refiner-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/refiner-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Survey your SaaS users with in-app micro-surveys that capture NPS, feature feedback, and churn signals at the perfect moment.

## Description
Connect your **Refiner** customer feedback account to any AI agent and simplify how you collect in-product insights, manage user segments, and monitor survey performance through natural conversation.

### What you can do

- **Survey Oversight** — List all in-app, email, and link surveys and retrieve detailed status and response counts.
- **Response Analysis** — Query survey submissions with technical filters like UUIDs and date ranges to identify trends.
- **Identity & Targeting** — Identify users and upsert technical traits to ensure surveys reach the right audience.
- **Event-Driven Feedback** — Track high-fidelity user actions programmatically to trigger perfectly timed micro-surveys via AI.
- **Segment Intelligence** — List and query defined user segments to understand your audience distribution.
- **Operational Monitoring** — Check API health and verify account configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Refiner API Key (found in your project settings)
3. Start managing your feedback ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check survey results and user sentiment via simple AI commands.
- **Growth & Marketing** — automate event tracking and verify segment metadata directly from the workspace.
- **Customer Success** — monitor individual user feedback and verify identity traits via the AI assistant.


## Available Tools
- **list_refiner_contacts**: List product contacts
- **get_refiner_contact**: Get contact details
- **identify_refiner_user**: Identify or update user
- **list_refiner_responses**: List survey responses
- **list_refiner_segments**: List user segments
- **check_refiner_status**: Check API Status
- **list_refiner_surveys**: List feedback surveys
- **track_refiner_event**: Track user event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refiner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my feedback surveys in Refiner."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 3 active surveys: 'NPS - Post Checkout', 'Beta Feedback', and 'New User Onboarding'. Which one would you like to see response counts or details for?

---

**👤 You:**
> "Show me the last 5 responses for the 'NPS - Post Checkout' survey."

**🤖 AI Agent:**
> I've fetched the latest responses. You have 5 recent submissions with scores ranging from 8 to 10. Users mentioned the 'speed of delivery' as a major positive. Shall I retrieve the full text for those responses?

---

**👤 You:**
> "Track event 'Clicked Upgrade' for user 'mike@example.com'."

**🤖 AI Agent:**
> Event tracked! I've logged 'Clicked Upgrade' for mike@example.com in Refiner. If you have any micro-surveys targeted to this event, they will be triggered for the user automatically.


## Installation & Usage

To install and use the **Refiner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/refiner](https://vinkius.com/mcp/refiner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
