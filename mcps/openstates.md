# OpenStates MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openstates)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openstates-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openstates-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

US state legislative data platform — track bills, legislators, and committees via AI.

## Description
Equip your AI agent with the most comprehensive US state-level legislative intelligence via **OpenStates**. This unified server provides your agent with instant access to bills, legislators, and committee metadata across all 50 states, DC, and Puerto Rico. Your agent can instantly search for specific legislation, audit legislator profiles, and retrieve committee memberships without you ever manually checking a government site. Whether you are tracking policy trends or verifying legislative actions, your agent acts as a dedicated political analyst through natural conversation.

### What you can do

- **Bill Discovery** — Search for thousands of legislative bills by keyword, jurisdiction, and session.
- **Legislator Auditing** — Fetch complete profiles, contact information, and current roles for state legislators.
- **Committee Intelligence** — List all legislative committees in a jurisdiction and retrieve their detailed membership lists.
- **Jurisdiction Lookup** — List and inspect all supported states and jurisdictions to understand current legislative coverage.
- **Deep Metadata** — Retrieve detailed actions and versions for specific bills to analyze the legislative process.

### How it works

1. Subscribe to this server
2. Enter your OpenStates API Key
3. Start managing your legislative intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Advocacy & Policy Teams** — instantly monitor relevant bills and track legislator stances across different states.
- **Journalists & Researchers** — retrieve historical legislative data and committee memberships for reporting and analysis.
- **IT & Civic Tech Developers** — integrate clean legislative data into transparency tools and public dashboards.
- **Citizens & Constituents** — stay updated on local legislative actions and find contact info for their representatives.
- **Legal Professionals** — verify the current status and versions of state-level legislation.


## Available Tools
- **get_bill_details**: Get bill details
- **get_committee_details**: Get committee details
- **get_legislator_details**: Get legislator details
- **list_committees**: List committees in a jurisdiction
- **list_jurisdictions**: List all jurisdictions
- **search_bills**: Search for legislative bills
- **search_legislators**: Search for legislators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenStates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for education bills in California."

**🤖 AI Agent:**
> Searching OpenStates for education-related bills in California... I've identified several active proposals, including AB-150 and SB-42. I can pull the full history and current status for any of these.

---

**👤 You:**
> "Who are the members of the New York Senate Finance Committee?"

**🤖 AI Agent:**
> Retrieving membership for the NY Senate Finance Committee... I've found 25 legislators currently serving on this committee, including the chair and vice-chair. Shall I list their names and parties for you?

---

**👤 You:**
> "Get the latest actions for bill TX HB-500."

**🤖 AI Agent:**
> Fetching details for Texas HB-500... The most recent action was 'Passed in the House' yesterday. It has now been referred to the Senate State Affairs committee. Would you like to see the full list of sponsors?


## Installation & Usage

To install and use the **OpenStates** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openstates](https://vinkius.com/mcp/openstates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
