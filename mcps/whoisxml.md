# WhoisXML MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whoisxml)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whoisxml-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whoisxml-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Access comprehensive domain intelligence, WHOIS records, IP geolocation, and email verification directly from your AI agent.

## Description
Connect the **WhoisXML API** to your AI agent to perform deep network reconnaissance and data validation through natural language.

### What you can do

- **WHOIS Lookups** — Retrieve parsed and raw registration data, including registrar info and creation dates for any domain.
- **IP Geolocation** — Instantly identify the country, city, ISP, and coordinates of any IP address.
- **Email Verification** — Validate email syntax, check MX records, and detect disposable addresses to ensure data quality.
- **Domain Availability** — Perform lightweight checks to see if a domain name is available for registration.

### How it works

1. Subscribe to this server
2. Enter your WhoisXML API Key
3. Start querying domain and network data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Researchers** — Quickly investigate suspicious domains or IP addresses during incident response.
- **Developers** — Integrate domain availability and email validation checks into your workflow without leaving the editor.
- **Marketers & Sales** — Verify lead lists and research company domain ownership for better outreach.


## Available Tools
- **check_domain_availability**: Check if a domain name is available for registration
- **get_ip_geolocation**: Get location data for an IP address
- **get_whois_record**: Get parsed and raw WHOIS data for a domain
- **verify_email**: Check if an email address is valid and exists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhoisXML** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the WHOIS record for google.com."

**🤖 AI Agent:**
> I've retrieved the WHOIS data for google.com. It was registered via MarkMonitor Inc. on 1997-09-15 and is set to expire on 2028-09-14.

---

**👤 You:**
> "Where is the IP address 8.8.8.8 located?"

**🤖 AI Agent:**
> The IP address 8.8.8.8 is located in Mountain View, California, United States. It is operated by Google LLC.

---

**👤 You:**
> "Verify if the email test@example.com is valid."

**🤖 AI Agent:**
> I checked test@example.com. The syntax is valid, but the domain does not have active MX records, suggesting it cannot receive emails.


## Installation & Usage

To install and use the **WhoisXML** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whoisxml](https://vinkius.com/mcp/whoisxml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
