# DNSimple MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dnsimple)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage domains, DNSSEC, and email forwarding via DNSimple — list accounts, control domains, and manage DS records directly from your AI agent.

## Description
Connect your **DNSimple** account to any AI agent to automate your domain infrastructure and DNS management through natural language.

### What you can do

- **Domain Management** — List all domains in your account, create new ones, or retrieve detailed metadata for existing domains.
- **DNSSEC Control** — Enable, disable, or check the status of DNSSEC for any domain to ensure cryptographic security.
- **DS Records** — Manage Delegation Signer (DS) records with tools to list, create, retrieve, and delete them for advanced DNS configurations.
- **Email Forwarding** — List, create, and inspect email forwarding rules to manage your communication flow without leaving your agent.
- **Account Identity** — Quickly identify the authenticated entity and list all accessible accounts and their IDs.

### How it works

1. Subscribe to this server
2. Enter your DNSimple API Token
3. Start managing your domains from Claude, Cursor, or any MCP-compatible client

Your AI acts as a specialized DevOps assistant, handling complex DNS operations with precision and speed.

### Who is this for?

- **DevOps Engineers** — automate domain provisioning and DNSSEC configurations directly from the terminal or chat.
- **Web Developers** — check domain statuses and manage email forwards without switching to the DNSimple dashboard.
- **IT Administrators** — audit multiple accounts and list domains across different organizational units efficiently.


## Available Tools (77)
- **accept_push**: Accept a domain push
- **activate_zone_dns**: Activate DNS for a zone
- **authorize_transfer_out**: Authorize domain transfer out
- **batch_change_zone_records**: Batch change zone records
- **change_domain_delegation**: Change name servers for a domain
- **check_domain_availability**: Check domain availability
- **check_zone_distribution**: Check zone distribution
- **check_zone_record_distribution**: Check zone record distribution
- **create_contact**: Create a contact
- **create_domain**: Create a domain in an account
- **create_ds_record**: Create a DS record for a domain
- **create_email_forward**: Create an email forward for a domain
- **create_template**: Create a template
- **create_webhook**: Create a webhook
- **create_zone_record**: Create a record in a zone
- **deactivate_zone_dns**: Deactivate DNS for a zone
- **dedelegate_from_vanity**: Dedelegate from vanity name servers
- **delegate_to_vanity**: Delegate to vanity name servers
- **delete_contact**: Delete a contact
- **delete_domain**: Delete a domain
- **delete_ds_record**: Delete a DS record
- **delete_email_forward**: Delete an email forward
- **delete_template**: Delete a template
- **delete_webhook**: Delete a webhook
- **delete_zone_record**: Delete a zone record
- **disable_auto_renewal**: Disable auto-renewal
- **disable_dnssec**: Disable DNSSEC for a domain
- **disable_whois_privacy**: Disable WHOIS privacy
- **download_certificate**: Download a certificate
- **enable_auto_renewal**: Enable auto-renewal
- **enable_dnssec**: Enable DNSSEC for a domain
- **enable_whois_privacy**: Enable WHOIS privacy
- **get_certificate_private_key**: Get private key for a certificate
- **get_certificate**: Retrieve a certificate
- **get_contact**: Retrieve a contact
- **get_dnssec**: Get DNSSEC status for a domain
- **get_domain_delegation**: List name servers for a domain
- **get_domain_prices**: Retrieve domain prices
- **get_domain**: Retrieve a domain
- **get_ds_record**: Retrieve a DS record
- **get_email_forward**: Retrieve an email forward
- **get_service**: Retrieve a service
- **get_template**: Retrieve a template
- **get_tld_extended_attributes**: Retrieve extended attributes for a TLD
- **get_tld**: Retrieve a TLD
- **get_webhook**: Retrieve a webhook
- **get_whoami**: Get details about the current authenticated entity
- **get_zone_file**: Download a zone file
- **get_zone_record**: Retrieve a zone record
- **get_zone**: Retrieve a zone
- **initiate_push**: Initiate a domain push
- **issue_letsencrypt_certificate**: Issue a Let's Encrypt certificate
- **list_accounts**: List accounts the authenticated entity has access to
- **list_zone_records**: List records in a zone
- **order_letsencrypt_renewal**: Order a Let's Encrypt certificate renewal
- **register_domain**: Register a domain
- **reject_push**: Reject a domain push
- **renew_domain**: Renew a domain
- **restore_domain**: Restore a domain
- **transfer_domain**: Transfer a domain
- **update_contact**: Update a contact
- **update_template**: Update a template
- **update_zone_record**: Update a zone record
- **issue_letsencrypt_renewal**: Issue a Let's Encrypt certificate renewal
- **list_billing_charges**: List billing charges for an account
- **list_certificates**: List certificates for a domain
- **list_contacts**: List contacts in an account
- **list_domains**: List domains in an account
- **list_ds_records**: List DS records for a domain
- **list_email_forwards**: List email forwards for a domain
- **list_pending_pushes**: List pending domain pushes
- **list_services**: List services
- **list_templates**: List templates in an account
- **list_tlds**: List TLDs
- **list_webhooks**: List webhooks in an account
- **list_zones**: List zones in an account
- **order_letsencrypt_certificate**: Order a Let's Encrypt certificate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DNSimple** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all domains in my DNSimple account 12345."

**🤖 AI Agent:**
> I've retrieved the domains for account 12345. You have 3 domains: 'example.com', 'my-app.io', and 'test-site.net'. Would you like details on any of these?

---

**👤 You:**
> "Enable DNSSEC for the domain 'example.com' in account 12345."

**🤖 AI Agent:**
> Processing... DNSSEC has been successfully enabled for 'example.com' in account 12345. You can verify the status anytime using the get_dnssec tool.

---

**👤 You:**
> "Show me the email forwarding rules for 'my-app.io' in account 9876."

**🤖 AI Agent:**
> I found 2 email forwarding rules for 'my-app.io': 'info@my-app.io' -> 'admin@gmail.com' and 'support@my-app.io' -> 'help@zendesk.com'.


## ❓ FAQ

**Q: How can I check if DNSSEC is enabled for a specific domain?**
You can use the `get_dnssec` tool by providing the Account ID and the Domain name. The agent will return the current DNSSEC status and details.

**Q: Can I list all domains across all my DNSimple accounts?**
First, use `list_accounts` to see all available Account IDs. Then, use `list_domains` with each specific Account ID to retrieve the domains associated with that account.

**Q: Is it possible to manage email forwarding rules through this agent?**
Yes! You can use `list_email_forwards` to see existing rules or `create_email_forward` to set up a new one for a specific domain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dnsimple](https://vinkius.com/mcp/dnsimple)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DNSimple** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dnsimple` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DNSimple** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dnsimple": {
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
