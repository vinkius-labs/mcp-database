# U.S. Congress MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-congress)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-congress-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-congress-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query U.S. legislative data via AI — search bills, members, amendments, treaties, nominations, committees, and congressional records.

## Description
Connect the **U.S. Congress API** to your AI agent and access comprehensive legislative data through natural conversation.

### What you can do

- **Bill Research** — Search and browse bills across congressional sessions with full text and status tracking
- **Member Lookup** — List current and past members of Congress with biographical and voting data
- **Amendment Tracking** — Browse amendments to bills and resolutions
- **Treaty Analysis** — Access treaty submissions and their current status
- **Nomination Tracking** — Monitor presidential nominations through the confirmation process
- **Committee Navigation** — Browse congressional committees and their jurisdictions
- **Congress History** — Access session data across historical congresses

### How it works

1. Subscribe to this server
2. Get a free API key from [Congress.gov](https://api.congress.gov/sign-up/)
3. Start researching legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Researchers** — quickly find bills, track their progress, and analyze legislative trends
- **Journalists** — research congressional activity, member records, and committee hearings
- **Civic Tech Developers** — build apps that make legislative data accessible to citizens


## Available Tools
- **get_bill_details**: Get full details for a specific legislative bill
- **list_congress_amendments**: List legislative amendments
- **list_congress_bills**: gov database.

List bills from the current or specified Congress
- **list_congress_committees**: List congressional committees
- **list_congress_sessions**: g., 118th, 117th) and their start and end dates.

List historical congressional sessions
- **list_congress_members**: List current or past members of the US Congress
- **list_congress_nominations**: List executive and judicial nominations
- **list_congress_treaties**: List treaties handled by Congress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Congress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What bills about artificial intelligence were introduced in the current Congress?"

**🤖 AI Agent:**
> Found 12 bills mentioning 'artificial intelligence' in the 118th Congress. Notable: H.R.6580 'AI Accountability Act' (referred to committee), S.3312 'Responsible AI Act' (passed Senate committee). Want details on any specific bill?


## Installation & Usage

To install and use the **U.S. Congress** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-congress](https://vinkius.com/mcp/us-congress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
