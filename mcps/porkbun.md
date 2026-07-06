# Porkbun MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/porkbun)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage domains and DNS records via Porkbun — list domains, update DNS, check pricing, and retrieve SSL certificates directly from your AI agent.

## Description
Connect your **Porkbun** account to any AI agent and take full control of your domain portfolio and DNS infrastructure through natural conversation.

### What you can do

- **Domain Management** — List all domains currently registered and managed in your Porkbun account.
- **DNS Control** — Create, edit, and delete DNS records (A, MX, CNAME, TXT, etc.) for any of your domains.
- **Pricing & Availability** — Check the availability of new domain names and get current pricing for all supported TLDs.
- **SSL Certificates** — Retrieve SSL certificate bundles for domains generated via Porkbun's automated systems.
- **Record Auditing** — Quickly retrieve and inspect all DNS records for a specific domain to troubleshoot configuration issues.

### How it works

1. Subscribe to this server
2. Enter your Porkbun API Key and Secret Key
3. Start managing your domains from Claude, Cursor, or any MCP-compatible client

No more logging into web consoles just to update a simple TXT record or check if a domain is available. Your AI acts as your personal domain administrator.

### Who is this for?

- **DevOps Engineers** — automate DNS record updates and verify infrastructure settings directly from the terminal or chat.
- **Web Developers** — check domain availability and pricing for new projects without breaking your development flow.
- **Domain Investors** — quickly list and monitor your entire portfolio and TLD pricing trends.


## Available Tools (8)
- **edit_dns_record**: Edit an existing DNS record
- **get_domain_pricing**: Get domain pricing information
- **list_domains**: List all domains in your account
- **retrieve_dns_records**: Retrieve all DNS records for a specific domain
- **retrieve_ssl_bundle**: Retrieve the SSL certificate bundle for a domain
- **check_domain_availability**: Check if a domain is available for registration
- **create_dns_record**: ) to the specified domain.

Create a new DNS record for a domain
- **delete_dns_record**: Delete a DNS record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Porkbun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all domains in my Porkbun account."

**🤖 AI Agent:**
> I've retrieved your domain list. You currently have 3 domains: 'myawesomeapp.com', 'dev-testing.net', and 'portfolio.io'. Which one would you like to manage?

---

**👤 You:**
> "Add a TXT record to 'example.com' with the value 'v=spf1 include:_spf.google.com ~all'."

**🤖 AI Agent:**
> I've successfully created the TXT record for 'example.com'. The record has been added with the SPF value provided. It may take some time to propagate globally.

---

**👤 You:**
> "Check the pricing for .com and .net domains."

**🤖 AI Agent:**
> Fetching current Porkbun pricing... For .com domains, the registration/renewal price is $10.37/year. For .net domains, it is $11.48/year. Would you like to check availability for a specific name?


## ❓ FAQ

**Q: Can I see all DNS records for a domain at once?**
Yes! Use the `retrieve_dns_records` tool with your domain name. It will return a complete list of all active records including A, CNAME, MX, and TXT entries.

**Q: Is it possible to check if a domain is available for purchase?**
Absolutely. Use the `check_domain_availability` tool to query any domain name. The agent will tell you if it's available for registration.

**Q: Can I delete a DNS record if I made a mistake?**
Yes. Use the `delete_dns_record` tool by providing the domain and the specific record ID. This will permanently remove the record from Porkbun's nameservers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/porkbun](https://vinkius.com/mcp/porkbun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Porkbun** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `porkbun` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Porkbun** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "porkbun": {
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
