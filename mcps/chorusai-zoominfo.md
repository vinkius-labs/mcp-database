# Chorus.ai (ZoomInfo) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chorusai-zoominfo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chorusai-zoominfo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chorusai-zoominfo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Analyze sales conversations and meetings via Chorus.ai — track transcripts, identify key moments, and monitor team performance directly from any AI agent.

## Description
Connect your **Chorus.ai (ZoomInfo)** account to any AI agent and take full control of your conversation intelligence through natural conversation. Streamline how you review and coach your sales team's interactions.

### What you can do

- **Meeting Oversight** — List and retrieve details for all recorded meetings and calls natively
- **Transcription Intelligence** — Access full text transcripts for any engagement to review customer dialogue flawlessly
- **Moment Analysis** — Retrieve AI-identified key moments, such as next steps or pain points, securely
- **Team Management** — List all users and team members to manage access and review performance flawlessly
- **Engagement Visibility** — Monitor active and past engagements to understand sales cycle progress in real-time
- **Market Insights** — List tracked competitors mentioned in conversations to identify market trends flawlessly
- **Shared Knowledge** — Access shared meeting playlists to facilitate team learning directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chorus.ai API Token (obtained from Personal Settings)
3. Start managing your conversation intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — review team meetings and identify coaching opportunities using natural language
- **Account Executives** — quickly look up previous call transcripts and AI-identified moments without opening the dashboard
- **Revenue Ops** — audit meeting volumes and competitor mentions straight from their chat interface
- **Product Managers** — verify customer feedback and pain points discussed in sales calls


## Available Tools
- **get_my_chorus_profile**: Retrieve information about the currently authenticated session
- **get_meeting_details**: Get detailed information for a specific meeting
- **get_meeting_moments**: Retrieve AI-identified key moments for a meeting
- **get_meeting_transcript**: Retrieve the full text transcript for a meeting
- **list_tracked_competitors**: List competitors being tracked in conversations
- **list_chorus_meetings**: ai.

List recent meetings and calls
- **list_meeting_playlists**: List all shared meeting playlists
- **list_chorus_users**: List all users and team members in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chorus.ai (ZoomInfo)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my meetings from today in Chorus.ai."

**🤖 AI Agent:**
> Retrieving today's meetings... I found 3 recordings: 'Intro Call with Acme', 'Q2 Review - Global Corp', and 'Product Feedback Session'. All are fully processed and transcribed.

---

**👤 You:**
> "What were the key moments in the 'Intro Call with Acme'?"

**🤖 AI Agent:**
> Checking AI moments for the Acme call... I identified 4 key moments: 2 Next Steps (Follow up next Tuesday), 1 Competitor Mention (referencing 'Competitor X'), and 1 Pricing Discussion.

---

**👤 You:**
> "Who are the members of the 'EMEA Sales' team?"

**🤖 AI Agent:**
> Retrieving user list... I found 5 members in the EMEA Sales group: Sarah Miller (Team Lead), Mike Scott, John Doe, Jane Smith, and Bob Black.


## Installation & Usage

To install and use the **Chorus.ai (ZoomInfo)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chorusai-zoominfo](https://vinkius.com/mcp/chorusai-zoominfo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
