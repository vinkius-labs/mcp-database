# Decodo (Smartproxy) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/decodo-smartproxy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Decodo (formerly Smartproxy) network infrastructure — list proxy endpoints, monitor bandwidth, and fetch residential proxy configurations with your AI.

## Description
Connect your **Decodo (Smartproxy)** account to any AI agent to control your proxy endpoints, audit infrastructure, and track SERP/scraping data seamlessly. Interact with your server architecture and networking limits using natural language without jumping out of your IDE.

### What you can do

- **Inventory Management** — Effortlessly pull a list of active `list_proxy_endpoints`, `list_datacenter_proxies`, and `list_residential_proxies`
- **Live Bandwidth Monitoring** — Run `get_traffic_usage` directly inside the AI prompt to see if you are about to hit your monthly data quota cap
- **Bot Statistics** — Evaluate the health of your bots automatically by checking `get_scraper_stats` for eCommerce and SERP scrapers
- **Reselling & Accounts** — Generate your `list_subscriptions` details, retrieve your general account health, or list all nested sub-users associated with the account

### How it works

1. Subscribe to this server
2. Enter your Smartproxy (Decodo) API Key
3. Start using Claude, Cursor, or any MCP-compatible client to query your IP pools

Stop clicking through multiple dashboard pages just to copy-paste your internal proxy endpoint port. Let your agent do it programmatically.

### Who is this for?

- **Data Engineers & Scrapers** — pull the precise endpoint metrics, load stats on failure rates, and check if your pools are active while drafting crawler scripts
- **Network Admins** — list assigned dedicated networks (`list_dedicated_proxies`) to diagnose potential rate-limiting errors from CLI
- **SaaS Operators** — monitor sub-user metrics and their localized bandwidth usage effortlessly


## Available Tools (9)
- **get_account_details**: Retrieves Smartproxy account information
- **list_proxy_endpoints**: Lists available proxy endpoints
- **list_residential_proxies**: Lists residential proxy configurations
- **list_sub_users**: Lists all proxy sub-users
- **get_scraper_stats**: Retrieves statistics for scraping APIs
- **get_traffic_usage**: Retrieves traffic usage statistics
- **list_datacenter_proxies**: Lists datacenter proxy configurations
- **list_dedicated_proxies**: Lists dedicated proxy assignments
- **list_subscriptions**: Lists active proxy subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Decodo (Smartproxy)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all of our active datacenter proxy endpoints."

**🤖 AI Agent:**
> Here are the Datacenter Proxy Endpoints bound to your subscription:
- US-East Pool (hostname: `gate.dc.smartproxy.com:20000`)
- EU-Central Pool (hostname: `gate.dc.smartproxy.com:20001`)

Both are operational. Would you like me to insert snippet usage into a Python Request block?

---

**👤 You:**
> "Use Decodo and query my scraping success rate summary."

**🤖 AI Agent:**
> Running a stat check using the get_scraper_stats module...

- API Hits Total: 4,025 requests
- Successful: 3,901 (96.9% rate)
- Blocked/Timeout: 124 (3.1% rate)
Your Google SERP APIs are performing excellently right now.

---

**👤 You:**
> "Have we exceeded the traffic usage on the account?"

**🤖 AI Agent:**
> Checking your subscription details...
You have a total cap of 100 GB. Current usage reflects 78.4 GB used (78% of your overall allocation). 
You are completely safe for now, with roughly 21.6 GB left this billing cycle.


## ❓ FAQ

**Q: Can the AI generate a script with my actual proxy endpoints already inserted?**
Yes. While prompting inside an IDE like Cursor, you can ask 'Write a Python script using my residential proxy endpoint.' The AI agent will call `list_residential_proxies` in the background, harvest the legit port numbers, and assemble runnable code on the spot.

**Q: Is it safe to pull network architecture metrics inside Claude AI?**
Absolutely secure. The MCP protocol bridges interactions locally. At no setup phase does Vinkius cloud servers retrieve your Smartproxy metrics directly—the exchange passes via your local agent bridging right into Decodo's endpoint.

**Q: Can it tell me my remaining bandwidth limit?**
Yes. Ask the bot 'How much target data do I have left?' and it will orchestrate the results of both `get_account_details` (which returns quota details) and `get_traffic_usage` (which exposes used data) to compute the remaining bytes in conversational form.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decodo-smartproxy](https://vinkius.com/mcp/decodo-smartproxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Decodo (Smartproxy)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `decodo-smartproxy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Decodo (Smartproxy)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "decodo-smartproxy": {
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
