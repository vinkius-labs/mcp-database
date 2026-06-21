# WhoisXML MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whoisxml)
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


## ❓ FAQ

**Q: Can I check if a domain is available for registration?**
Yes! Use the `check_domain_availability` tool. It provides a lightweight check to see if a specific domain name is currently available.

**Q: How do I find the physical location of an IP address?**
Simply use the `get_ip_geolocation` tool with the target IP. The agent will return the country, city, latitude, longitude, and ISP information.

**Q: Can this tool detect disposable or fake email addresses?**
Yes. The `verify_email` tool checks email syntax, MX records, and SMTP connections, and specifically flags disposable email providers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whoisxml](https://vinkius.com/mcp/whoisxml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WhoisXML** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `whoisxml` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WhoisXML** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whoisxml": {
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
