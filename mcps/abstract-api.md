# Abstract API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abstract-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enrich and verify data — audit geolocation, emails, and VAT via AI.

## Description
Empower your AI agent to orchestrate your entire data enrichment and verification workflow with **Abstract API**, the comprehensive platform for global data intelligence. By connecting Abstract API to your agent, you transform complex validation tasks into a natural conversation. Your agent can instantly geolocate IP addresses, audit email deliverability, and retrieve VAT company details without you ever touching a manual verification tool. Whether you are conducting market analysis or verifying user identity, your agent acts as a real-time data steward, ensuring your intelligence is always grounded in verified, high-quality data.

### What you can do

- **Geolocation Auditing** — Geolocate any IP address and retrieve detailed metadata, including city, country, and ISP information.
- **Email Oversight** — Verify email addresses to maintain strict control over deliverability and avoid bounce rates instantly.
- **Business Intelligence** — Validate VAT numbers and retrieve comprehensive company profiles for compliance and due diligence.
- **Financial Intelligence** — Query real-time exchange rates between any currency pairs to monitor market trends.
- **Global Monitoring** — List public holidays and retrieve current timezone data for any location to coordinate international operations.

### How it works

1. Subscribe to this server
2. Enter your Abstract API Key
3. Start managing your data intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — monitor user geolocation and retrieve identity metadata straight from your workflow.
- **Compliance Officers** — verify VAT numbers and audit corporate profiles without manual database searches.
- **Marketers** — perform rapid audits of email lists and validate lead quality through natural language.
- **Operations Leads** — automate global data querying to orchestrate cross-functional international teams smoothly.


## Available Tools (6)
- **get_exchange_rate**: Get current exchange rates between two currencies
- **get_holidays**: List public holidays for a country and year
- **get_timezone**: Get current time and timezone details for a location
- **validate_vat**: Validate a VAT number and retrieve company details
- **validate_email**: Verify if an email address is valid and deliverable
- **geolocate_ip**: Get geographic details for an IP address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Abstract API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geolocate the IP address 8.8.8.8 using Abstract API."

**🤖 AI Agent:**
> I've geolocated the IP! It is located in Mountain View, California, United States. The ISP is identified as Google. Would you like the full geographic metadata?

---

**👤 You:**
> "Validate the email address 'test@vinkius.com'."

**🤖 AI Agent:**
> Email validated! The address is deliverable and has a high confidence score. It is not a disposable email. Would you like me to check another address?

---

**👤 You:**
> "What are the public holidays in 'BR' for 2024?"

**🤖 AI Agent:**
> I've retrieved the public holidays for Brazil in 2024. Notable dates include Carnival on February 13th and Independence Day on September 7th. I can provide the full list if you'd like.


## ❓ FAQ

**Q: How do I find my Abstract API Key?**
Log in to your [**Abstract API dashboard**](https://app.abstractapi.com/), select the API you want to use, and you will find your API Key on the settings page. Copy and paste it below.

**Q: Can the agent check if an email is real?**
Yes. Use the `validate_email` tool providing the email address. Your agent will return a deliverability score and identify if the address is a disposable or role-based email.

**Q: Is it possible to validate international VAT numbers?**
Yes. The `validate_vat` tool allows your agent to verify VAT numbers for businesses across multiple jurisdictions, primarily in Europe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abstract-api](https://vinkius.com/mcp/abstract-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Abstract API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `abstract-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Abstract API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abstract-api": {
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
