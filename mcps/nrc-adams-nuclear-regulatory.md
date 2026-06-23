# NRC ADAMS (Nuclear Regulatory) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nrc-adams-nuclear-regulatory)
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


## Available Tools (2)
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


## ❓ FAQ

**Q: How can I search for specific technical documents like 'Gamma Knife' in the NRC library?**
You can use the `search_adams_legacy` tool. Provide a query string in the `q` parameter, such as `(mode:sections,sections:(filters:(public-library:!t),single_content_search:'Gamma+Knife'))`, to filter for documents in the public library.

**Q: Is it possible to get the daily operational status of nuclear power plants?**
Yes. Use the `get_nrc_rss_feed` tool and set the `feed` parameter to `plant-status`. This will retrieve the latest power reactor status reports directly from the NRC.

**Q: What happens to the search functionality after June 2026?**
The `search_adams_legacy` tool uses the WBA API which is scheduled for retirement in June 2026. After this date, the server will need to be updated to support the NRC's successor API systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nrc-adams-nuclear-regulatory](https://vinkius.com/mcp/nrc-adams-nuclear-regulatory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NRC ADAMS (Nuclear Regulatory)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nrc-adams-nuclear-regulatory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NRC ADAMS (Nuclear Regulatory)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nrc-adams-nuclear-regulatory": {
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
