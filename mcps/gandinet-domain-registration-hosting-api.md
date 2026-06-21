# Gandi.net (Domain Registration & Hosting API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gandinet-domain-registration-hosting-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Gandi.net domains, DNS records, mailboxes, and hosting instances directly from your AI agent.

## Description
Connect your **Gandi.net** account to any AI agent to automate domain management, DNS configuration, and hosting oversight through natural language.

### What you can do

- **Domain Management** — List all registered domains, fetch detailed metadata, and check real-time availability for new registrations.
- **LiveDNS Control** — Full CRUD operations on DNS records (A, CNAME, TXT, etc.) to manage your infrastructure's routing without leaving your chat or IDE.
- **Email Administration** — List and create mailboxes, and manage email aliases for any of your managed domains.
- **Hosting & Infrastructure** — Monitor your Gandi hosting instances and retrieve technical details for your web deployments.
- **Organization Insights** — Access information about the organizations and billing entities associated with your account.

### How it works

1. Subscribe to this server
2. Enter your Gandi.net API Key (v5)
3. Start managing your web presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly update DNS records or check hosting status during deployments.
- **Web Developers** — verify domain availability and set up mailboxes for clients directly from the code editor.
- **IT Administrators** — audit domain portfolios and organization access across multiple Gandi entities.


## Available Tools
- **check_domain**: Check if a domain is available for registration
- **create_dns_record**: Create a new DNS record for a domain
- **create_mailbox**: Create a new mailbox for a domain
- **delete_dns_record**: Delete a DNS record
- **get_domain**: Get detailed information about a specific domain
- **get_hosting_instance**: Get details for a specific Simple Hosting instance
- **get_organization**: Get details for a specific organization
- **list_aliases**: List aliases for a specific mailbox
- **list_dns_records**: List all DNS records for a domain
- **list_domains**: List domains associated with your Gandi account
- **list_hosting_instances**: List all Simple Hosting instances
- **list_mailboxes**: List all mailboxes for a given domain
- **list_organizations**: List organizations you belong to
- **update_dns_record**: Update an existing DNS record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gandi.net (Domain Registration & Hosting API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all domains in my Gandi account."

**🤖 AI Agent:**
> I've retrieved your domain list. You have 3 domains: 'example.com', 'my-portfolio.net', and 'dev-site.org'. Would you like more details on any of these?

---

**👤 You:**
> "Check if 'cool-new-app.io' is available for registration."

**🤖 AI Agent:**
> Checking availability for 'cool-new-app.io'... Good news! The domain is currently available for registration. Would you like to know the next steps?

---

**👤 You:**
> "Show me the DNS records for 'example.com'."

**🤖 AI Agent:**
> Fetching DNS records for 'example.com'... I found 4 records: an A record pointing to 93.184.216.34, two MX records for mail, and a TXT record for verification. Do you need to modify any of these?


## ❓ FAQ

**Q: Can I check if a domain is available for registration using this tool?**
Yes! Use the `check_domain` tool with the FQDN you're interested in. The agent will return the availability status directly from Gandi's registry.

**Q: How do I update a DNS record for one of my domains?**
You can use the `update_dns_record` tool. You'll need to provide the domain (fqdn), the record name (like 'www'), the type (like 'A'), and the new record data in JSON format.

**Q: Can I see my hosting instances and their status?**
Absolutely. Use the `list_hosting_instances` tool to get an overview of all your hosting services, or `get_hosting_instance` for detailed information on a specific one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gandinet-domain-registration-hosting-api](https://vinkius.com/mcp/gandinet-domain-registration-hosting-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gandi.net (Domain Registration & Hosting API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gandinet-domain-registration-hosting-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gandi.net (Domain Registration & Hosting API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gandinet-domain-registration-hosting-api": {
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
