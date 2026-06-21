# Chameleon.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chameleonio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chameleonio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chameleonio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage product adoption and onboarding via Chameleon — trigger tours, analyze surveys, and track user events directly from any AI agent.

## Description
Connect your **Chameleon.io** account to any AI agent and take full control of your user onboarding and product adoption experiences through natural conversation. Streamline how you guide and engage your users.

### What you can do

- **Experience Oversight** — List and retrieve details for all Chameleon tours, launchers, and microsurveys natively
- **User Segmentation** — Access and monitor your configured user segments to understand targeting flawlessly
- **Response Auditing** — Retrieve and analyze recent microsurvey responses to gather user feedback securely
- **User Intelligence** — Identify and update user profiles with custom properties in real-time
- **Behavioral Tracking** — Log and monitor custom user events to trigger the right experience at the right time flawlessly
- **Compliance Management** — Handle data deletion requests by removing user records directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chameleon Account Secret (obtained from Settings > API)
3. Start managing your product experiences from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor onboarding health and review survey feedback using natural language
- **Product Marketing Managers** — audit active experiences and segments without opening the dashboard
- **Customer Success Managers** — identify and track user behaviors to improve engagement straight from their chat interface
- **Developers** — verify event tracking and user identification data during integration


## Available Tools
- **delete_chameleon_user**: Permanently delete a user and their data from Chameleon
- **get_experience_details**: Get details for a specific experience
- **identify_chameleon_user**: Identify or update a user in Chameleon
- **list_chameleon_events**: List recent events tracked by Chameleon
- **list_experiences**: List all Chameleon experiences (Tours, Launchers, Microsurveys)
- **list_user_segments**: List all configured user segments
- **list_microsurvey_responses**: List recent responses to microsurveys
- **track_user_event**: Track a custom event for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chameleon.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Chameleon experiences."

**🤖 AI Agent:**
> Retrieving your active experiences... I found 5 active items: 'Welcome Home' (Tour), 'New Feature Alert' (Launcher), and 3 microsurveys. Which one would you like to inspect?

---

**👤 You:**
> "Identify user 'user_999' with plan: 'enterprise' and industry: 'fintech'."

**🤖 AI Agent:**
> Identifying user_999... The profile has been successfully updated in Chameleon with the provided properties. They will now be eligible for any experiences targeting the 'enterprise' plan.

---

**👤 You:**
> "Track a 'checkout_completed' event for user 'user_123'."

**🤖 AI Agent:**
> Tracking 'checkout_completed' for user_123... The event has been logged. If you have any experiences triggered by this event, they will now be displayed to the user.


## Installation & Usage

To install and use the **Chameleon.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chameleonio](https://vinkius.com/mcp/chameleonio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
