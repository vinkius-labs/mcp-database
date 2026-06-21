# AskNicely MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asknicely)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/asknicely-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/asknicely-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Manage customer experience and NPS surveys with AskNicely — track responses and audit sentiment via AI.

## Description
The **AskNicely MCP Server** provides a powerful natural language interface to your customer experience platform. Empower your AI agent to monitor your Net Promoter Score (NPS), retrieve real-time user feedback, and manage your contact survey workflows seamlessly.

### Key Capabilities

- **NPS Monitoring** — Retrieve your aggregate NPS statistics and track changes in customer sentiment over time.
- **Response Analysis** — Access detailed survey responses, including scores and customer comments, to identify pain points and success stories.
- **Contact Management** — List and audit your contact database, including when users were last surveyed.
- **Survey Automation** — Trigger new surveys for specific customers directly from your chat interface to capture immediate feedback.
- **Real-time Statistics** — Get instant summaries of your customer experience metrics without manual dashboard exports.
- **Secure API Access** — Uses your AskNicely API Key for safe and authenticated communication.

### Who is this for?

- **Customer Success Managers** — Quickly audit recent feedback from specific accounts or segments.
- **Product Managers** — Use AI-assisted summaries to understand user sentiment regarding new features or updates.
- **Marketing Teams** — Identify promoters for case studies and testimonials using natural language queries.


## Available Tools
- **get_account_check**: Verify AskNicely account connection
- **get_statistics**: Get aggregate NPS statistics and summary
- **list_contacts**: List contacts in your AskNicely account
- **list_responses**: List NPS survey responses from AskNicely
- **trigger_survey**: Add a contact and trigger a survey immediately


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AskNicely** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our current NPS statistics."

**🤖 AI Agent:**
> Your current Net Promoter Score is 72. You have 85 promoters, 10 passives, and 5 detractors in the last 30 days.

---

**👤 You:**
> "List the last 5 survey responses with comments."

**🤖 AI Agent:**
> I've retrieved the latest responses. The most recent comment from 'John Doe' says: 'Love the new interface, very intuitive!' with a score of 10.

---

**👤 You:**
> "Trigger an NPS survey for 'Jane Smith' at 'jane@example.com'."

**🤖 AI Agent:**
> The survey for Jane Smith (jane@example.com) has been successfully triggered and she has been added to your contacts.


## Installation & Usage

To install and use the **AskNicely** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asknicely](https://vinkius.com/mcp/asknicely)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
