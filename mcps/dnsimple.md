# DNSimple MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dnsimple)
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
- **activate_zone_dns**: Supply the account and zone names.

Activate DNS for a zone
- **check_domain_availability**: Provide the account ID and the domain name to check.

Check domain availability
- **delete_domain**: Delete a domain
- **get_certificate_private_key**: Provide the certificate ID.

Get private key for a certificate
- **get_contact**: Provide the Account ID and Contact ID.

Retrieve a contact
- **get_email_forward**: Use the account ID, domain, and the unique email forward ID.

Retrieve an email forward
- **get_whoami**: Get details about the current authenticated entity
- **list_templates**: Provide the account ID.

List templates in an account
- **list_zone_records**: Provide the account and zone name.

List records in a zone
- **reject_push**: Supply the account ID and the specific push ID.

Reject a domain push
- **create_domain**: Create a domain in an account
- **create_webhook**: Provide the account ID and the webhook payload.

Create a webhook
- **list_contacts**: Provide the Account ID.

List contacts in an account
- **check_zone_distribution**: Specify the account and zone name.

Check zone distribution
- **check_zone_record_distribution**: Supply the account, zone name, and record ID.

Check zone record distribution
- **create_contact**: Provide the Account ID and the contact payload.

Create a contact
- **create_ds_record**: Create a DS record for a domain
- **create_template**: Provide the account ID and the template payload.

Create a template
- **delegate_to_vanity**: Provide the account, domain, and the vanity payload.

Delegate to vanity name servers
- **delete_contact**: Provide both the account ID and the contact ID.

Delete a contact
- **delete_email_forward**: Specify the account ID, domain, and the email forward ID.

Delete an email forward
- **delete_template**: Delete a template
- **delete_webhook**: Provide the account ID and the webhook ID.

Delete a webhook
- **delete_zone_record**: Supply the account, zone name, and record ID.

Delete a zone record
- **disable_auto_renewal**: Specify the account and domain name.

Disable auto-renewal
- **disable_dnssec**: Disable DNSSEC for a domain
- **download_certificate**: Provide the certificate ID.

Download a certificate
- **enable_auto_renewal**: Specify the account and domain name.

Enable auto-renewal
- **enable_dnssec**: Enable DNSSEC for a domain
- **enable_whois_privacy**: Specify the account and domain name.

Enable WHOIS privacy
- **get_certificate**: Provide the certificate ID and domain.

Retrieve a certificate
- **get_dnssec**: Get DNSSEC status for a domain
- **get_domain_delegation**: Use the domain name or ID.

List name servers for a domain
- **get_domain_prices**: Supply the account ID and the domain name.

Retrieve domain prices
- **get_domain**: Retrieve a domain
- **get_ds_record**: Retrieve a DS record
- **get_service**: Pass the service ID.

Retrieve a service
- **get_tld_extended_attributes**: Pass the TLD name.

Retrieve extended attributes for a TLD
- **get_tld**: Supply the TLD name.

Retrieve a TLD
- **get_zone_record**: Supply the account, zone name, and record ID.

Retrieve a zone record
- **get_zone**: Provide both account and zone names.

Retrieve a zone
- **initiate_push**: Provide the account ID, domain, and the required push payload.

Initiate a domain push
- **issue_letsencrypt_certificate**: Provide the certificate ID to initiate the process.

Issue a Let's Encrypt certificate
- **list_accounts**: List accounts the authenticated entity has access to
- **list_billing_charges**: List billing charges for an account
- **list_certificates**: Specify the domain name or ID.

List certificates for a domain
- **list_email_forwards**: Provide the account ID and domain name.

List email forwards for a domain
- **list_services**: List services
- **list_tlds**: List TLDs
- **list_webhooks**: Specify the account ID.

List webhooks in an account
- **list_zones**: Only the account ID is required.

List zones in an account
- **order_letsencrypt_certificate**: Include the required domain and order payload.

Order a Let's Encrypt certificate
- **register_domain**: Provide the account ID, domain name, and the registration payload.

Register a domain
- **renew_domain**: The renewal payload must specify the desired period.

Renew a domain
- **restore_domain**: Provide the necessary restore payload.

Restore a domain
- **transfer_domain**: Supply the account ID, domain name, and the transfer payload.

Transfer a domain
- **update_contact**: Provide the Account ID, Contact ID, and new contact payload.

Update a contact
- **update_template**: Provide the account, template ID, and new body content.

Update a template
- **update_zone_record**: Supply the account, zone name, record ID, and new payload.

Update a zone record
- **accept_push**: Supply the account ID, push ID, and the acceptance payload.

Accept a domain push
- **authorize_transfer_out**: No additional parameters are required.

Authorize domain transfer out
- **batch_change_zone_records**: Provide the account, zone name, and batch payload.

Batch change zone records
- **change_domain_delegation**: Supply the account, domain, and the new delegation payload.

Change name servers for a domain
- **create_email_forward**: Supply the account ID, domain, and the forward payload.

Create an email forward for a domain
- **create_zone_record**: Supply the account, zone name, and the record payload.

Create a record in a zone
- **deactivate_zone_dns**: Supply the account and zone names.

Deactivate DNS for a zone
- **dedelegate_from_vanity**: Specify the account and domain name.

Dedelegate from vanity name servers
- **delete_ds_record**: Delete a DS record
- **disable_whois_privacy**: Specify the account and domain name.

Disable WHOIS privacy
- **get_template**: Retrieve a template
- **get_webhook**: Supply both the account ID and the webhook ID.

Retrieve a webhook
- **get_zone_file**: Supply the account and zone names.

Download a zone file
- **issue_letsencrypt_renewal**: Provide the renewal ID.

Issue a Let's Encrypt certificate renewal
- **list_domains**: List domains in an account
- **list_ds_records**: List DS records for a domain
- **list_pending_pushes**: Specify the Account ID to filter results.

List pending domain pushes
- **order_letsencrypt_renewal**: Provide the certificate ID and renewal payload.

Order a Let's Encrypt certificate renewal


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

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dnsimple](https://vinkius.com/en/ai-agent-connect/dnsimple)
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
