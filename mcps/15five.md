# 15Five MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/15five)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/15five-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/15five-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower performance management with 15Five — manage check-ins, high fives, objectives, and team feedback directly from your AI agent.

## Description
Transform your team’s engagement and performance with **15Five**, the holistic performance management platform now accessible through your AI agent. By bridging 15Five with the Model Context Protocol, you turn employee check-ins and objective tracking into a seamless conversation. Your agent can help you celebrate wins with High Fives, monitor team sentiment via Pulse scores, and audit OKRs without you ever leaving your primary workspace. It’s the ultimate tool for managers who want to stay connected to their team’s heartbeat while focusing on strategic growth.

### What you can do

- **Check-ins & Feedback** — Retrieve recent check-ins, view employee answers, and monitor pulse scores to gauge team sentiment.
- **High Fives & Recognition** — List received high fives or send new ones to celebrate team wins and boost morale directly from chat.
- **Objectives (OKRs)** — Track progress on company or individual objectives and key results without manual dashboard lookups.
- **User & Team Management** — List employees, departments, and groups to maintain organizational clarity.
- **Engagement Insights** — Quickly access historical performance data and feedback cycles to support meaningful 1-on-1 conversations.

### How it works

1. Subscribe to this server
2. Enter your 15Five API Key and Subdomain
3. Start managing performance and recognition through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **People Leaders & Managers** — stay updated on team check-ins and recognize achievements through simple commands
- **HR Professionals** — audit objectives and engagement levels across departments seamlessly
- **Team Members** — quickly view goals and send high fives to colleagues without context switching
- **Operations Teams** — automate data retrieval for performance reporting and organizational health monitoring


## Available Tools
- **list_users**: Use this to find the identifier for a person.

List all active employees and users in the 15Five organization
- **list_departments**: Useful for finding the department ID or identifying team structures.

List all departments and their members
- **list_checkins**: Use this to monitor team sentiment or review previous employee submissions. You can filter by user ID.

List recent employee check-ins and performance reports
- **list_high_fives**: List recent High Fives (public recognition) across the company
- **send_high_five**: Requires the email address of the recipient and a personal message.

Send a High Five to publicly recognize a colleague
- **list_objectives**: List company and individual objectives (OKRs)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **15Five** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 check-ins for my team."

**🤖 AI Agent:**
> I've retrieved the last 5 check-ins. You can see summaries from John, Sarah, and Alex, including their pulse scores and key challenges. Would you like to dive into a specific one?

---

**👤 You:**
> "Send a High Five to Sarah for her great work on the project."

**🤖 AI Agent:**
> High Five successfully sent to Sarah! She will receive a notification celebrating her contribution to the project. Anything else I can help with?

---

**👤 You:**
> "List all active company objectives."

**🤖 AI Agent:**
> I've listed the current company objectives. You have 3 active OKRs, with the 'Revenue Growth' target at 75% completion. Would you like a breakdown of the key results?


## Installation & Usage

To install and use the **15Five** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/15five](https://vinkius.com/mcp/15five)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
