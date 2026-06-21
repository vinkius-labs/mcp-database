# Local Falcon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/local-falcon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track your Google Maps rankings across geographic grids and monitor local SEO performance for every business location.

## Description
Connect your **Local Falcon** account to any AI agent and take full control of your local search visibility and automated rank tracking workflows through natural conversation.

### What you can do

- **Scan & Report Orchestration** — List and manage all completed high-fidelity scan reports programmatically, retrieving detailed geo-grid ranking data and competitor metrics
- **Real-Time Visibility Intelligence** — Programmatically trigger new geo-grid scans for specific keywords and locations to monitor your local search performance in real-time
- **Ranking Architecture** — Access high-fidelity metrics including ARP (Average Ranking Position), ATRP, and SoLV (Share of Local Voice) directly through your agent
- **Competitor Monitoring** — Access high-fidelity ranking data for local competitors at every grid point to coordinate your search optimization strategy
- **Operational Monitoring** — Verify account-level API connectivity and monitor scan credit usage directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Local Falcon dashboard (API Credentials section)
3. Start orchestrating your local SEO from Claude, Cursor, or any MCP client

No more manual checking of individual rank trackers or missing local visibility drops. Your AI acts as your dedicated local search coordinator and SEO architect.

### Who is this for?

- **SEO Managers** — instantly retrieve local ranking recaps and monitor SoLV trends using natural language commands
- **Agency Owners** — generate automated geo-grid reports and verify competitor performance without leaving your workspace
- **Marketing Operations** — automate the management of scheduled scans and campaign reporting through simple AI queries


## Available Tools (13)
- **add_keyword**: Add a keyword
- **add_location**: Add a location
- **check_localfalcon_status**: Verify connectivity
- **get_location**: Get location details
- **get_scan_report**: Get scan report
- **get_scan_results**: Get scan results
- **get_scan**: Get scan details
- **get_trend_report**: Get trend report
- **list_scans_by_location**: List scans by location
- **list_keywords**: List keywords
- **list_locations**: List locations
- **list_scans**: List scans
- **run_scan**: Run a new scan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Falcon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 scan reports in my Local Falcon account."

**🤖 AI Agent:**
> I've retrieved your scans. You currently have 50 completed reports, including 'Plumber SEO Grid' and 'Dental NYC'. Would you like the detailed high-fidelity ranking metadata for any of them?

---

**👤 You:**
> "Show the rankings and SoLV for scan report 'rep_123'."

**🤖 AI Agent:**
> Accessing ranking architecture... Report rep_123 shows an ARP of 3.5 and a Share of Local Voice (SoLV) of 65%. I've retrieved the high-fidelity grid data for your review. Need help analyzing your top competitors?

---

**👤 You:**
> "Run a new grid scan for business 'Acme Plumbers' and keyword 'emergency plumbing'."

**🤖 AI Agent:**
> Scan orchestrated! I've successfully triggered a new geo-grid scan for 'Acme Plumbers'. The report key is rep_456. Local Falcon is now gathering real-time visibility data. Shall I notify you once the high-fidelity results are ready?


## ❓ FAQ

**Q: How do I find my Local Falcon API Key?**
Log in to your account, navigate to the **API Credentials** page, and copy your unique Bearer Token or API Key.

**Q: Can I run new scans via AI?**
Yes! The `run_localfalcon_scan` tool allows your agent to trigger real-time geo-grid scans by providing business and keyword metadata.

**Q: How do I check my scan credit balance?**
Use the `check_localfalcon_status` tool to retrieve your current account metrics and remaining high-fidelity scan credits programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/local-falcon](https://vinkius.com/mcp/local-falcon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Falcon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-falcon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Falcon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-falcon": {
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
