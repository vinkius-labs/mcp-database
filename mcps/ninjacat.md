# NinjaCat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ninjacat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage marketing reporting and advertisers via NinjaCat — track reports, data sources, and campaigns directly from your AI agent.

## Description
Connect your **NinjaCat** agency account to your AI agent and streamline your marketing reporting and advertiser management through natural conversation.

### What you can do

- **Advertiser Management** — List all advertisers managed in your agency and retrieve detailed profiles and account information.
- **Report Oversight** — Access agency reports, monitor their execution history, and get direct download URLs for the latest generated files.
- **Data Source Tracking** — List all marketing platforms and connected data accounts (e.g., Google Ads, Facebook Ads) to monitor your ecosystem.
- **Campaign Monitoring** — View active marketing campaigns across the agency to stay on top of performance.
- **Agency Insights** — Retrieve high-level information and settings for your NinjaCat agency and current user profile.
- **Deep Inspection** — Fetch complete metadata for specific advertisers or reports using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your NinjaCat Agency Identifier Key, Client ID, and Client Secret
3. Start managing your marketing agency data from Claude, Cursor, or any MCP client

### Who is this for?

- **Agency Managers** — quickly check report statuses or advertiser details without navigating the NinjaCat portal.
- **Account Managers** — monitor campaign distribution and data source connectivity directly from your workspace.
- **Marketing Analysts** — automate the retrieval of report history and download links for performance audits.


## Available Tools
- **get_advertiser**: Get specific advertiser details
- **get_agency_info**: Get agency metadata
- **get_me**: Get current user details
- **get_report_download_url**: Get report download URL
- **get_report_history**: Get report execution history
- **list_data_accounts**: g. specific Google Ads accounts).

List connected data accounts
- **list_advertisers**: List all advertisers
- **list_agency_campaigns**: List agency marketing campaigns
- **list_data_sources**: List active data sources
- **list_reports**: List all agency reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NinjaCat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertisers in my NinjaCat agency."

**🤖 AI Agent:**
> Retrieving advertisers... I found 8 active clients, including 'Acme Corp', 'Global Retail Ltd', and 'Innovate Tech'. Would you like the detailed contact info for Acme Corp?

---

**👤 You:**
> "Show me the execution history for the 'Monthly Performance' report."

**🤖 AI Agent:**
> Fetching report history... The 'Monthly Performance' report (ID: rep_123) was last run successfully today at 8:00 AM. It has a history of 12 successful runs over the last year. Shall I get the download URL for the latest run?

---

**👤 You:**
> "Which marketing data sources are currently connected?"

**🤖 AI Agent:**
> Retrieving data sources... Your account is currently connected to 5 platforms: Google Ads, Meta Ads, LinkedIn Ads, GA4, and TikTok Ads. You have a total of 24 data accounts active across these sources. Would you like a list of the specific Google Ads accounts?


## ❓ FAQ

**Q: Where do I find my NinjaCat API credentials?**
Log in to your NinjaCat agency settings and navigate to the 'Apps' tab. There you will find your Agency Identifier Key, Client ID, and Client Secret.

**Q: Can I download a report directly through the agent?**
Yes! The `get_report_download_url` tool provides the direct link to the latest generated file for a specific report, allowing you to access it without opening the portal.

**Q: How do I see which data sources are connected?**
Use the `list_data_sources` tool to see all platforms (e.g., Google Ads, Facebook) integrated with your account, and `list_data_accounts` for specific account connections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ninjacat](https://vinkius.com/mcp/ninjacat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NinjaCat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ninjacat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NinjaCat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ninjacat": {
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
