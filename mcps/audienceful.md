# Audienceful MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/audienceful)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/audienceful-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/audienceful-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage subscribers, custom fields, and email automations via Audienceful — orchestrate newsletters and campaigns directly via AI.

## Description
Connect your **Audienceful** account to any AI agent and transform how you manage your email marketing and audience data through natural conversation.

### What you can do

- **People Management** — Create, search, and update subscriber profiles and manage their subscription status across your workspace
- **Custom Data Fields** — Define and manage custom data points to segment your audience with surgical precision
- **Automation Triggers** — Programmatically trigger email sequences and marketing automations for specific users or events
- **Performance Auditing** — Query and analyze campaign performance and audience growth metrics without manual exports

### How it works

1. Subscribe to this server
2. Enter your Audienceful API Key
3. Start managing your email marketing workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — instantly manage your newsletter subscribers and check growth stats while writing content
- **Marketing Teams** — trigger complex sequences and update user tags directly from your team's workspace
- **Growth Engineers** — automate the creation of custom fields and data mapping from your IDE


## Available Tools
- **create_custom_field**: Create a new custom field for your audience members
- **create_person**: You must provide at least an email address.

Add a new person to your audience
- **delete_custom_field**: Delete a custom field
- **delete_person**: Use with caution.

Permanently remove a person from your audience
- **get_person**: Get details for a specific person by their UID
- **list_custom_fields**: List all custom fields defined in your audience
- **list_people**: You can filter by status or search for a specific email address.

List all people in your Audienceful audience
- **list_send_reports**: List recent email send reports
- **trigger_automation**: Manually trigger an automation for a person
- **update_person**: Update an existing person profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audienceful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for subscribers who have the 'Company' field set to 'TechCorp'."

**🤖 AI Agent:**
> I've scanned your audience. I found 3 subscribers matching 'TechCorp': Sarah L. ([email protected]), Mike R. ([email protected]), and Anna K. ([email protected]). Would you like to tag them all with 'Enterprise'?

---

**👤 You:**
> "Trigger the 'onboarding-welcome' sequence for [email protected]"

**🤖 AI Agent:**
> The automation 'onboarding-welcome' has been successfully triggered for [email protected]. They should receive the first email in the sequence shortly.

---

**👤 You:**
> "List all custom fields currently defined in my Audienceful workspace."

**🤖 AI Agent:**
> I've retrieved your custom data structure. You currently have 5 custom fields defined: 'Company' (company_name), 'Job Title' (job_title), 'Lead Score' (lead_score), 'Referral Source' (ref_source), and 'Last Event' (last_event).


## Installation & Usage

To install and use the **Audienceful** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audienceful](https://vinkius.com/mcp/audienceful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
