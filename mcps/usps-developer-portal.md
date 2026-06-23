# USPS Developer Portal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usps-developer-portal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage US mail — audit addresses, tracking, and ZIP codes via AI.

## Description
Empower your AI agent to orchestrate your entire postal logistics and address auditing workflow with the **USPS Developer Portal**, the official source for United States Postal Service data. By connecting USPS Web Tools to your agent, you transform complex shipping tasks into a natural conversation. Your agent can instantly verify addresses, audit package tracking statuses, and retrieve ZIP code metadata without you ever touching a shipping portal. Whether you are managing e-commerce deliveries or conducting regional address audits, your agent acts as a real-time logistics consultant, ensuring your data is always verified and precise.

### What you can do

- **Address Auditing** — Standardize and verify United States addresses to ensure your shipping metadata is always grounded in official USPS records.
- **Advanced Tracking Control** — Track real-time package statuses and access granular facility-level tracking events instantly.
- **ZIP Code & Routing Discovery** — Cross-reference ZIP codes with city/state pairs to understand the geographic reach of your logistics.
- **Domestic & International Rates** — Accurately calculate the real-time cost of shipping across various mail classes, weights, and global destinations.
- **Service Delays & Commitments** — Query live delivery commitments by mail class to accurately orchestrate e-commerce fulfillment.

### How it works

1. Subscribe to this server
2. Enter your USPS Web Tools User ID
3. Start managing your postal intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — monitor package timelines and retrieve official metadata straight from your workflow.
- **E-commerce Leads** — verify customer addresses and audit delivery patterns without manual searching.
- **Address Researchers** — perform rapid audits of US locations and identify relevant ZIP markers through natural language.
- **Operations Leads** — automate postal data querying to orchestrate cross-functional shipping teams smoothly.


## Available Tools (8)
- **calculate_domestic_rate**: Calculate USPS domestic shipping rates
- **calculate_international_rate**: Calculate USPS international shipping rates
- **get_delivery_commitments**: Get USPS service delivery commitments and estimates
- **lookup_usps_city_state**: Look up the city and state for a ZIP code
- **lookup_usps_zip_code**: Look up the exact ZIP code for a specific US address
- **track_usps_package_advanced**: Get advanced tracking information for a USPS package
- **track_usps_package**: Track a USPS package using a tracking number
- **verify_usps_address**: Verify and standardize a US address using USPS Web Tools


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USPS Developer Portal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify address '1600 Pennsylvania Avenue NW, Washington, DC 20500' using USPS."

**🤖 AI Agent:**
> I've retrieved the verification metadata from USPS! The address is identified as valid and standardized. Would you like the full XML response or the ZIP+4 metadata for this location?

---

**👤 You:**
> "Track my package with tracking number '9400100000000000000000'."

**🤖 AI Agent:**
> I've checked the status for that tracking number. It is currently identified as 'Delivered' at [Time]. I can assist you with the full event history metadata for this shipment if you'd like.

---

**👤 You:**
> "Lookup ZIP code for 'Seattle, WA'."

**🤖 AI Agent:**
> I've retrieved the ZIP code metadata for Seattle! Notable codes include 98101 and 98104. I can provide the specific address-level ZIP details to assist in your regional logistics audit.


## ❓ FAQ

**Q: How do I find my USPS User ID?**
Register for an account at the [**USPS Web Tools registration page**](https://www.usps.com/business/web-tools-apis/welcome.htm). You will receive your User ID via email. Copy and paste it below.

**Q: Does it support international tracking?**
Yes. The `track_usps_package` tool supports tracking for any valid USPS tracking number, including international shipments originating from or delivered by USPS.

**Q: What is the format for address verification?**
The API requires an object with line1, city, and state metadata. Standardizing these inputs ensures the most accurate verification from the USPS database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usps-developer-portal](https://vinkius.com/mcp/usps-developer-portal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USPS Developer Portal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `usps-developer-portal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USPS Developer Portal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usps-developer-portal": {
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
