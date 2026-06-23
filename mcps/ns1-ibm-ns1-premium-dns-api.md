# NS1 (IBM NS1 Premium DNS API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ns1-ibm-ns1-premium-dns-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage DNS zones, records, and traffic steering via IBM NS1. Automate infrastructure directly from your AI agent.

## Description
Connect your **IBM NS1** account to any AI agent and take full control of your global DNS infrastructure and traffic steering through natural conversation.

### What you can do

- **Zone Management** — List, create, update, and delete DNS zones (domains) managed in your NS1 account.
- **Record Control** — Manage DNS records (A, CNAME, TXT, etc.) with support for complex answers and TTL configurations.
- **Traffic Steering** — Configure filters and answers for advanced traffic management and global load balancing.
- **Monitoring & Health** — List and create monitoring jobs to track endpoint health across various global regions.
- **Data Feeds** — Manage data sources and push real-time data feeds to drive dynamic DNS responses.

### How it works

1. Subscribe to this server
2. Enter your NS1 API Key
3. Start managing your network infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — instantly update DNS records or check monitoring statuses without leaving the terminal or IDE.
- **Cloud Architects** — orchestrate complex traffic steering configurations and global load balancing via simple prompts.
- **Infrastructure Teams** — automate the provisioning of new zones and records as part of CI/CD workflows.


## Available Tools (15)
- **create_data_source**: Create a new data source
- **create_monitoring_job**: Create a new monitoring job
- **create_record**: Create a new DNS record
- **create_zone**: Create a new DNS zone
- **delete_record**: Delete a DNS record
- **delete_zone**: Delete a DNS zone
- **get_record**: Get details for a specific DNS record
- **get_zone**: Get details for a specific zone
- **list_data_sources**: List all data sources
- **list_monitoring_jobs**: List all monitoring jobs
- **list_monitoring_regions**: List available monitoring regions
- **list_zones**: List all DNS zones
- **push_data_feed**: Push data to a specific feed
- **update_record**: Update an existing DNS record
- **update_zone**: Update zone settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NS1 (IBM NS1 Premium DNS API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my DNS zones in NS1."

**🤖 AI Agent:**
> I've retrieved your zones. You currently manage 3 zones: 'production.com', 'staging.net', and 'api-gateway.io'. Which one would you like to manage?

---

**👤 You:**
> "Create an A record for 'www.production.com' pointing to '1.2.3.4' with a TTL of 3600."

**🤖 AI Agent:**
> I've successfully created the A record for 'www.production.com' in the 'production.com' zone. It is now pointing to 1.2.3.4 with a TTL of 3600 seconds.

---

**👤 You:**
> "Show me all active monitoring jobs and their regions."

**🤖 AI Agent:**
> Fetching monitoring data... I found 2 active jobs: 'Global-Web-Check' (monitoring from US-East, EU-West, and Asia-Pacific) and 'API-Health' (monitoring from US-West).


## ❓ FAQ

**Q: Can I create a new DNS zone using this server?**
Yes! Use the `create_zone` tool with the zone name (e.g., 'example.com'). You can also optionally set TTL, refresh, and expiry values during creation.

**Q: How do I add a record with specific answers for traffic steering?**
Use the `create_record` tool. You can provide a JSON array of `answers` (e.g., IP addresses) and a JSON array of `filters` to define how NS1 should steer traffic between those answers.

**Q: Can I see my active monitoring jobs and their status?**
Yes, the `list_monitoring_jobs` tool retrieves all configured monitoring jobs, allowing your AI agent to report on the health and status of your monitored endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ns1-ibm-ns1-premium-dns-api](https://vinkius.com/mcp/ns1-ibm-ns1-premium-dns-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NS1 (IBM NS1 Premium DNS API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ns1-ibm-ns1-premium-dns-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NS1 (IBM NS1 Premium DNS API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ns1-ibm-ns1-premium-dns-api": {
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
