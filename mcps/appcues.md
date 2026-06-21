# Appcues MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appcues)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/appcues-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/appcues-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your Appcues flows, segments, and user experiences with AI — track activity and publish content effortlessly.

## Description
The **Appcues MCP Server** empowers your AI agent to interact directly with your Appcues account. Whether you need to audit your current onboarding flows, manage user segments, or track real-time user activity, this integration provides a seamless natural language interface to your product experience platform.

### Key Features

- **Flow Management** — List, view, publish, and unpublish flows (in-app experiences) across web and mobile.
- **User Segmentation** — Retrieve and analyze your targeting segments to understand who is seeing your content.
- **Activity Tracking** — Send real-time events and profile updates for immediate targeting and personalization.
- **Mobile Support** — Access specific experiences designed for your mobile applications.
- **Auditing & Reporting** — Quickly check account status, checklists, and experience metadata.

### Benefits for Teams

- **Product Managers** — Quickly audit which onboarding flows are active and make changes without leaving your AI workspace.
- **Growth Engineers** — Programmatically track user events to trigger personalized in-app journeys.
- **Customer Success** — View user profiles and segment membership to provide better support and guidance.


## Available Tools
- **get_account_details**: Verify Appcues account connection
- **get_flow**: Get details for a specific flow
- **get_segment**: Get details for a specific segment
- **get_user_profile**: Retrieve the profile of a specific user
- **list_checklists**: List all checklists configured in the account
- **list_flows**: List all Appcues flows (experiences) for the account
- **list_mobile_experiences**: List mobile-specific experiences
- **list_segments**: List all user segments defined in Appcues
- **publish_flow**: Publish a draft flow
- **track_user_activity**: Use JSON strings for profileUpdate and events.

Track real-time events and profile updates for a user
- **unpublish_flow**: Unpublish an active flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appcues** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Appcues flows."

**🤖 AI Agent:**
> I've retrieved your flows. You have 5 active flows, including 'New User Onboarding', 'Feature Announcement v2', and 'NPS Survey'.

---

**👤 You:**
> "Track a 'clicked_checkout' event for user 'user_123'."

**🤖 AI Agent:**
> The 'clicked_checkout' event has been successfully tracked for user 'user_123'.

---

**👤 You:**
> "Show me the details of the segment with ID '998877'."

**🤖 AI Agent:**
> Segment '998877' is named 'High Value Customers' and currently contains 1,250 users.


## Installation & Usage

To install and use the **Appcues** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appcues](https://vinkius.com/mcp/appcues)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
