# vote.direct MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/votedirect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/votedirect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/votedirect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage voter info — audit polling locations, elections, and registration via IA.

## Description
Empower your AI agent to orchestrate your entire civic participation and voter auditing workflow with **vote.direct**, the comprehensive source for localized election data. By connecting vote.direct to your agent, you transform complex voter searches into a natural conversation. Your agent can instantly search for polling locations, audit upcoming elections, and retrieve registration deadlines without you ever touching a government portal. Whether you are preparing for a local vote or conducting regional civic research, your agent acts as a real-time civic consultant, ensuring your data is always verified and localized.

### What you can do

- **Polling Auditing** — Search for polling locations near any street address and retrieve detailed metadata, including hours and names.
- **Election Oversight** — Audit upcoming elections for specific ZIP codes to maintain a clear view of local civic timelines and scale.
- **Ballot Discovery** — Retrieve detailed ballot information for specific elections to understand the legislative items and candidates instantly.
- **Registration Intelligence** — Query voter registration deadlines and links for any state to assist in civic compliance and planning.
- **Civic Monitoring** — Check API status to ensure your civic research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your vote.direct API Key
3. Start managing your civic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Civic Engagement Leads** — monitor voter timelines and retrieve localized metadata straight from your workflow.
- **Political Researchers** — verify polling distribution and audit registration patterns without manual searching.
- **Voters & Volunteers** — perform rapid audits of local ballots and identify registration links through natural language.
- **Operations Leads** — automate civic data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **check_api_status**: direct election data service.

Check if the vote.direct service is operational
- **get_ballot_information**: Get ballot information for a specific election and address
- **get_upcoming_elections**: Find upcoming elections for a specific ZIP code
- **get_polling_locations**: Find polling locations near a specific address
- **get_registration_details**: Get voter registration deadlines and links for a specific state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vote.direct** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find polling locations near '1600 Pennsylvania Avenue NW, Washington, DC' using vote.direct."

**🤖 AI Agent:**
> I've retrieved the polling locations for that address! The nearest site is identified as [Name], located at [Address]. It is open from 7 AM to 8 PM on election day. Would you like to see other nearby locations?

---

**👤 You:**
> "What elections are upcoming for ZIP code '90210'?"

**🤖 AI Agent:**
> I've identified 2 upcoming elections for 90210! These include a Municipal Election on June 4th and a General Election on November 5th. I can provide the ballot details for either if you'd like.

---

**👤 You:**
> "Get registration deadline for 'New York'."

**🤖 AI Agent:**
> I've retrieved the registration information for New York. The deadline for online registration is 15 days before the election. I can provide the official registration link to assist you with the process.


## Installation & Usage

To install and use the **vote.direct** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/votedirect](https://vinkius.com/mcp/votedirect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
