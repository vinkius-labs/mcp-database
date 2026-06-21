# Residential Proxies MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/residential-proxies)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Route web traffic through residential IP addresses worldwide for scraping, testing, and research that avoids blocks and captchas.

## Description
Connect your **AppVidLab Residential Proxies** account to any AI agent and take full control of your automated web data collection and proxy rotation workflows through natural conversation.

### What you can do

- **Proxy Pool Orchestration** — List and manage your entire high-fidelity database of working residential proxies programmatically, retrieving detailed IP and port technical metadata
- **Geo-Targeting Intelligence** — Programmatically query and monitor proxies from specific countries to coordinate your international data mining strategy in real-time
- **Rotation Architecture** — Access high-fidelity rotating IP strings to maintain a perfectly coordinated audit trail of your scraping sessions and bypass bot detection
- **Availability Monitoring** — Access real-time status updates and track proxy health directly through your agent for instant operational reporting
- **Infrastructure Verification** — Verify account-level API connectivity and monitor proxy usage directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **RapidAPI Key** from your RapidAPI dashboard (AppVidLab Residential Proxies API section)
3. Start orchestrating your data collection from Claude, Cursor, or any MCP client

No more manual copy-pasting of proxy strings or missing connectivity drops. Your AI acts as your dedicated network coordinator and data architecture architect.

### Who is this for?

- **Data Engineers** — instantly retrieve proxy lists and monitor rotation health using natural language commands
- **Web Scrapers** — verify geo-targeting metadata and track proxy availability without leaving your creative workspace
- **Growth Leads** — integrate high-speed residential proxy data into custom data extraction pipelines through simple AI queries


## Available Tools (10)
- **check_proxy_status**: Verify Residential Proxies API connectivity
- **get_proxy_count**: Get the total number of available proxies
- **get_br_proxies**: Get Brazil residential proxies
- **get_proxies_by_country**: g., US, GB, DE, BR).

Get residential proxies filtered by country
- **get_de_proxies**: Get Germany residential proxies
- **get_proxies_limited**: Useful for testing or sampling available proxies.

Get a limited number of proxies
- **get_uk_proxies**: Get United Kingdom residential proxies
- **get_us_proxies**: Get United States residential proxies
- **list_proxies**: List all available residential proxies
- **get_multi_country_proxies**: Returns a summary with counts and sample proxies per country.

Get proxies from multiple countries at once


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Residential Proxies** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List 10 working residential proxies from the USA."

**🤖 AI Agent:**
> I've retrieved the proxies. I found 10 high-fidelity working IPs from the US, formatted as IP:Port:User:Pass. Would you like the detailed latency metadata for any of them?

---

**👤 You:**
> "Show available residential proxies for country code 'GB'."

**🤖 AI Agent:**
> Accessing proxy intelligence... For country code GB, I've identified 15 high-fidelity working residential proxies. I've retrieved the technical metadata for your scraping session. Need help monitoring the availability status?

---

**👤 You:**
> "Check my RapidAPI status and proxy usage metrics."

**🤖 AI Agent:**
> Operational monitoring complete! Your API connection to RapidAPI is active and healthy. Your account has processed 1,000 high-fidelity proxy requests this month. Shall I retrieve the detailed usage breakdown?


## ❓ FAQ

**Q: How do I find my RapidAPI Key?**
Log in to [**RapidAPI**](https://rapidapi.com/), navigate to the AppVidLab Residential Proxies API page, and copy your unique API Key from the endpoints section.

**Q: Can I target specific countries via AI?**
Yes! The `list_working_proxies` tool supports a `country_code` parameter to retrieve high-fidelity proxies from specific locations.

**Q: Are the proxies rotating?**
Yes, the API provides high-fidelity residential IP strings that rotate to ensure anonymity and maintain technical scraping performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/residential-proxies](https://vinkius.com/mcp/residential-proxies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Residential Proxies** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `residential-proxies` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Residential Proxies** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "residential-proxies": {
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
