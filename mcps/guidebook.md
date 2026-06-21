# Guidebook MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidebook)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guidebook-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guidebook-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate mobile app content management via Guidebook — manage guides, sessions, speakers, and custom lists directly from any AI agent.

## Description
Connect your **Guidebook Builder** account to any AI agent and manage your mobile event or organization app content through natural conversation.

### What you can do

- **Guide Oversight** — List all mobile guides in your account and retrieve detailed metadata for each.
- **Schedule Management** — Browse, list, and inspect schedule sessions to keep your event timeline up to date.
- **Speaker Coordination** — Access speaker profiles and presenter details to ensure all bio information is accurate.
- **Custom Lists** — Manage Exhibitors, Sponsors, or any other custom data lists within your app.
- **Venue & Locations** — Retrieve all defined locations and map data for your event.
- **Rate Limit Tracking** — Monitor your API usage to stay within your daily quota.

### How it works

1. Subscribe to this server
2. Enter your Guidebook API Key (JWT token)
3. Start managing your app content from Claude, Cursor, or any MCP-compatible client

No more manual data entry in the Builder interface. Your AI assistant acts as a dedicated content coordinator for your mobile apps.

### Who is this for?

- **Event Organizers** — quickly verify session times and speaker assignments without digging through the CMS.
- **Content Managers** — automate the retrieval and auditing of custom lists like exhibitors or sponsors.
- **App Developers** — integrate Guidebook content flows into your development environment seamlessly.


## Available Tools
- **get_guide**: Get detailed information about a specific guide
- **get_rate_limit**: Check current API usage and rate limits
- **get_session**: Get details for a specific schedule session
- **get_speaker**: Get details for a specific speaker profile
- **list_custom_lists**: List custom list items (e.g., Exhibitors, Sponsors) for a guide
- **list_guides**: List all guides available in the account
- **list_locations**: List all locations/venues defined for a guide
- **list_schedules**: List schedules for a specific guide
- **list_sessions**: List all schedule sessions for a specific guide
- **list_speakers**: List all speakers/presenters for a specific guide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guidebook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active mobile guides in my account."

**🤖 AI Agent:**
> I've retrieved your guides. You have 3 active projects: 'Global Tech Summit 2024' (ID: 8821), 'Internal Sales Kickoff' (ID: 8825), and 'Partner Conference Q2' (ID: 8830). Which guide would you like to inspect?

---

**👤 You:**
> "Show the schedule sessions for guide ID 8821."

**🤖 AI Agent:**
> Fetching sessions for Guide 8821... I found 5 main sessions for today, including 'Opening Keynote' at 09:00 AM, 'Cloud Infrastructure Workshop' at 11:30 AM, and 'Networking Lunch' at 01:00 PM. Should I get more details on any of these?

---

**👤 You:**
> "Who are the speakers for the Global Tech Summit?"

**🤖 AI Agent:**
> Accessing speakers for Guide 8821... I've identified 12 profiles, including Dr. Sarah Chen (AI Research), Marcus Viera (DevOps Lead), and Jane Doe (UX Design). Would you like to see a specific speaker's full bio?


## Installation & Usage

To install and use the **Guidebook** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidebook](https://vinkius.com/mcp/guidebook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
