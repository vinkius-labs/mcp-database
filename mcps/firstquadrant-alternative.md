# FirstQuadrant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firstquadrant-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firstquadrant-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firstquadrant-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Orchestrate AI-driven sales and marketing campaigns. Manage API keys, user registration, and campaign execution directly through your AI agent.

## Description
FirstQuadrant is an advanced platform for AI-driven outreach and campaign management. This MCP server allows you to integrate FirstQuadrant's powerful automation capabilities directly into your AI workflows.

### What you can do

- **Campaign Management** — List, create, update, and execute marketing campaigns to drive growth and engagement.
- **API Key Orchestration** — Manage the full lifecycle of API keys, including creation, rotation, and deletion for secure programmatic access.
- **User & Auth Control** — Register new users and manage authentication sessions seamlessly within your organizational environment.
- **Execution Control** — Trigger specific campaign runs and monitor status in real-time to ensure your outreach is performing as expected.

### How it works

1. Subscribe to this server
2. Enter your FirstQuadrant API Key
3. Start managing your sales automation and campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — Launch and monitor campaigns without leaving your workspace.
- **Sales Ops** — Manage API keys and user registrations for automated outreach tools.
- **Developers** — Integrate FirstQuadrant capabilities into custom AI agents for automated lead generation.


## Available Tools
- **archive_contact**: Archive a contact
- **count_contacts**: Count contacts
- **create_api_key**: Create a new API key
- **create_auth**: Create or refresh an access token
- **create_campaign_sequence**: Create a new sequence for a campaign
- **create_campaign**: Create a new campaign
- **create_campaign_variant**: Create a new variant for a campaign
- **create_company**: Create a new company
- **create_contact**: Create a new contact
- **create_deal**: Create a new deal
- **create_pipeline**: Create a new pipeline
- **create_variant_step**: Create a new step for a variant
- **delete_api_key**: Delete an API key
- **delete_auth**: Log out to end an authenticated session
- **delete_campaign**: Delete a campaign
- **delete_contact**: Delete a contact
- **enrich_company**: Enrich a company
- **enrich_contact**: Enrich a contact with external data
- **export_contacts**: Export contacts
- **get_api_key**: Get an API key
- **get_auth**: Get authentication details
- **get_campaign**: Get a campaign
- **get_campaigns_analytics**: Aggregate analytics for campaigns
- **get_company**: Get a company
- **get_contact**: Get a contact
- **get_deal**: Get a deal
- **get_deals_analytics**: Aggregate analytics for deals
- **get_health**: Verify the service is running
- **get_logs**: Access system logs
- **get_resource**: Retrieve a generic resource by ID
- **get_usage**: Get organization usage statistics
- **hard_stop_campaign**: Hard stop a campaign
- **list_api_keys**: List API keys
- **list_campaign_sequences**: List sequences for a campaign
- **list_campaign_variants**: List variants for a campaign
- **list_campaigns**: List campaigns
- **list_companies**: List companies
- **list_company_employees**: List employees of a company
- **list_connections**: List active integrations
- **list_contacts**: List contacts
- **list_deals**: List deals
- **list_generations**: List AI generations
- **list_pipeline_stages**: List stages in a pipeline
- **list_pipelines**: List pipelines
- **list_variant_steps**: List steps for a variant
- **receive_hubspot_webhook**: Receive HubSpot webhook events
- **receive_nylas_webhook**: Receive Nylas webhook events
- **receive_stripe_webhook**: Receive Stripe webhook events
- **regenerate_api_key**: Regenerate an API key
- **regenerate_campaign_sequences**: Regenerate all sequences for a campaign
- **register_user**: Register a new user
- **replace_api_key**: Replace an API key
- **replace_campaign**: Replace a campaign
- **run_campaign**: Run a campaign
- **sequence_campaign**: Sequence a campaign
- **update_api_key**: Update an API key
- **update_campaign**: Update a campaign
- **update_contact**: Update a contact
- **update_deal**: Update a deal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FirstQuadrant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active campaigns in FirstQuadrant."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Q4 Outreach' (ID: camp_001), 'Lead Nurturing' (ID: camp_002), and 'Re-engagement' (ID: camp_003).

---

**👤 You:**
> "Run the campaign with ID camp_001."

**🤖 AI Agent:**
> Starting campaign 'Q4 Outreach' (camp_001) now. I will monitor the execution status for you.

---

**👤 You:**
> "Generate a new API key for my development environment."

**🤖 AI Agent:**
> I've created a new API key for you. The ID is 'key_dev_99' and it is now ready for use in your development environment.


## Installation & Usage

To install and use the **FirstQuadrant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firstquadrant-alternative](https://vinkius.com/mcp/firstquadrant-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
