# NRC ADAMS (Nuclear Regulatory) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nrc-adams-nuclear-regulatory)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nrc-adams-nuclear-regulatory-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nrc-adams-nuclear-regulatory-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Access official Nuclear Regulatory Commission (NRC) documents, news, and reactor status reports directly through the ADAMS database.

## Description
Connect to the **NRC ADAMS** (Agencywide Documents Access and Management System) to query the primary repository for official records and public documents from the U.S. Nuclear Regulatory Commission.

### What you can do

- **Legacy Document Search** — Utilize the Web-Based ADAMS (WBA) API to search for publicly available documents using complex filters (Note: Legacy API retires June 2026).
- **Real-time Monitoring** — Fetch live RSS feeds for daily event reports, news releases, and current power reactor status.
- **Content Discovery** — Track new content additions to the NRC library as they are published.
- **Plant Status Tracking** — Monitor the operational status of nuclear power plants across the country through dedicated status feeds.

### How it works

1. Subscribe to this server
2. Enter your NRC API access credentials or identifier
3. Start querying nuclear regulatory data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — quickly find technical documents and safety reports related to nuclear materials and facilities.
- **Legal & Compliance Officers** — track regulatory filings, news releases, and official NRC correspondence.
- **Energy Analysts** — monitor daily plant status and event reports to understand trends in the nuclear power sector.


## Available Tools
- **get_nrc_rss_feed**: Get NRC RSS feeds for events, news, and status
- **search_adams_legacy**: Note: This API is retiring June 2026. The q parameter uses a complex filter structure.

Search NRC ADAMS documents using the legacy WBA API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NRC ADAMS (Nuclear Regulatory)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search NRC ADAMS for public documents related to 'Gamma Knife' technology."

**🤖 AI Agent:**
> I am searching the ADAMS legacy database... I found several documents including safety evaluations and licensing records for Gamma Knife facilities. Would you like to see the specific document titles and dates?

---

**👤 You:**
> "Get the latest NRC news releases and announcements."

**🤖 AI Agent:**
> Fetching the NRC news feed... The latest updates include a new regulatory guide release and an upcoming public meeting regarding reactor safety oversight. Should I summarize the top three stories?

---

**👤 You:**
> "Show me the current daily power reactor status report."

**🤖 AI Agent:**
> Retrieving plant status... I have the daily report showing power levels and operational status for all commercial nuclear units. Most plants are operating at 100% power, with two units currently in scheduled refueling outages.


## Installation & Usage

To install and use the **NRC ADAMS (Nuclear Regulatory)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nrc-adams-nuclear-regulatory](https://vinkius.com/mcp/nrc-adams-nuclear-regulatory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
