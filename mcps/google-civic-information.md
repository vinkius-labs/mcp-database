# Google Civic Information MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-civic-information)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage political data — audit representatives and elections via AI.

## Description
Empower your AI agent to orchestrate your entire civic participation and political auditing workflow with **Google Civic Information**, the authoritative source for localized government data. By connecting Google's civic intelligence to your agent, you transform complex political searches into a natural conversation. Your agent can instantly identify your representatives, audit upcoming elections, and retrieve detailed polling metadata without you ever touching a government portal. Whether you are conducting regional policy research or preparing for a local vote, your agent acts as a real-time civic consultant, ensuring your data is always verified and precise.

### What you can do

- **Representative Auditing** — Search for political officials by street address and retrieve comprehensive metadata, including names, parties, and office titles.
- **Election Oversight** — Audit upcoming and past elections to maintain a clear view of civic timelines and scale.
- **Voter Intelligence** — Query polling locations and ballot information for specific addresses to assist in civic preparation.
- **Division Discovery** — Search for electoral divisions (OCD-IDs) by name or location to understand regional administrative reach instantly.
- **Civic Monitoring** — Check API status to ensure your political research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Google Civic Information API Key
3. Start managing your civic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Political Analysts & Researchers** — monitor official data and retrieve representative metadata straight from your workflow.
- **Civic Engagement Leads** — verify polling locations and audit election timelines without manual searching.
- **Voters & Journalists** — perform rapid audits of political officials and identify relevant civic markers through natural language.
- **Operations Leads** — automate civic data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **check_api_status**: Check if the Google Civic Information API is operational
- **get_google_civic_elections**: List upcoming and past elections supported by Google Civic
- **get_representatives_by_address**: Find political representatives for a specific street address
- **get_voter_information**: Get voter information (polling sites, ballots) for an address and election
- **search_civic_divisions**: Search for electoral divisions (OCD-IDs) by name or location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Civic Information** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are my political representatives for '1600 Pennsylvania Avenue NW, Washington, DC'?"

**🤖 AI Agent:**
> I've retrieved the representatives for that address! Notable officials include the President of the United States and Congressional representatives from the District of Columbia. I can provide the party affiliation and office titles for each if you'd like.

---

**👤 You:**
> "Search for civic divisions related to 'Chicago'."

**🤖 AI Agent:**
> I've identified several electoral divisions for Chicago! These include the City of Chicago and Cook County. I can provide the OCD-IDs for these divisions to assist in further representative audits.

---

**👤 You:**
> "What elections are upcoming in the United States?"

**🤖 AI Agent:**
> I've retrieved the election catalog from Google Civic! Notable upcoming events include state primaries and the next General Election. I can provide the unique election IDs and dates for each of these if you'd like.


## ❓ FAQ

**Q: How do I find my Google Civic API Key?**
Log in to the [**Google Cloud Console**](https://console.cloud.google.com/), create a project, enable the 'Google Civic Information API', and generate an API Key in the 'Credentials' section. Copy and paste it below.

**Q: Can the agent identify state-level representatives?**
Yes. The `get_representatives_by_address` tool retrieves officials at federal, state, and local levels based on the provided address metadata.

**Q: Does it support polling location search?**
Yes. Use the `get_voter_information` tool providing an address and optionally an election ID to retrieve official polling site metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-civic-information](https://vinkius.com/mcp/google-civic-information)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Civic Information** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-civic-information` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Civic Information** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-civic-information": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
