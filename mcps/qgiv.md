# Qgiv MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qgiv)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Manage Qgiv donation forms, custom fields, suggested amounts, and account settings directly from any AI agent.

## Description
Connect your **Qgiv** account to any AI agent to streamline your nonprofit fundraising workflows. Manage donation forms, customize suggested amounts, configure custom fields, and update account settings through natural conversation.

### What you can do

- **Form Cloning** — Quickly clone existing donation forms to launch new campaigns in seconds.
- **Account & Form Settings** — Retrieve and update organization-level and form-level settings, including custom form wording.
- **Custom Suggested Amounts** — List, retrieve, create, and update suggested donation amounts to optimize donor giving tiers.
- **Custom & Dedication Fields** — Manage custom fields and dedication options on your donation forms to collect vital donor information.

### How it works

1. Subscribe to this server
2. Enter your Qgiv API Token
3. Start managing your fundraising forms and settings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nonprofit Administrators** — Easily update donation form settings, custom wording, and suggested amounts without navigating complex dashboards.
- **Fundraising Campaign Managers** — Clone successful donation forms instantly to launch new seasonal or emergency campaigns.
- **Operations Teams** — Audit and maintain custom fields and dedication options across all active forms.


## Available Tools
- **clone_form**: Clone an existing form
- **create_custom_amount**: Create custom suggested donation amounts
- **create_custom_field**: Create custom fields on donation forms
- **create_dedication_field**: Create custom dedication fields
- **create_dedication_type**: Create dedication types
- **create_kiosk**: Create a new kiosk
- **create_pledge**: Create pledges
- **create_report_mapping**: Create report mappings
- **create_restriction**: Create fund restrictions
- **get_account_settings**: Get organization and form-level settings
- **get_custom_amount**: Get a specific custom amount by ID
- **get_custom_field**: Get a specific custom field by ID
- **get_dedication_field**: Get a specific dedication field by ID
- **get_dedication_type**: Get a specific dedication type by ID
- **get_event**: Get a specific event by ID
- **get_form_wording**: Get custom wording on organization forms
- **get_kiosk**: Get a specific kiosk by ID
- **get_last_refunds**: Get the last N refunds
- **get_last_registrations**: Get the last N Peer-to-Peer registrations
- **get_last_transactions**: Get the last N transactions
- **get_latest_statement**: Get the latest financial statement
- **get_pledge**: Get a specific pledge by ID
- **get_recurring_profile**: Get a specific recurring profile by ID
- **get_refund**: Get a specific refund by ID
- **get_refunds_after**: Get refunds after a specific Refund ID
- **get_refunds_by_dates**: Get refunds by date range
- **get_registration**: Get a specific Peer-to-Peer registration by ID
- **get_registrations_by_dates**: Get Peer-to-Peer registrations by date range
- **get_report_mapping**: Get a specific report mapping by ID
- **get_restriction**: Get a specific restriction by ID
- **get_statement**: Get a specific statement by ID
- **get_transactions_after**: Get transactions after a specific Transaction ID
- **get_transactions_by_dates**: Get transactions by date range
- **get_widget**: Get a specific widget by ID
- **list_custom_amounts**: List custom suggested donation amounts
- **list_custom_fields**: List custom fields on donation forms
- **list_dedication_fields**: List custom dedication fields
- **list_dedication_types**: List dedication types (e.g., In Honor Of)
- **list_events**: List custom events and ticket packages
- **list_kiosks**: List kiosk settings and navigation menus
- **list_pledges**: List pledges
- **list_recurring_profiles_by_status**: List recurring donation profiles by status
- **list_recurring_profiles**: List all recurring donation profiles
- **list_report_mappings**: List report mappings for third-party integrations
- **list_restrictions**: List fund restrictions (designations)
- **list_statements**: List financial statements and payout summaries
- **list_widgets**: List custom widgets associated with forms
- **update_account_settings**: Update organization and form-level settings
- **update_custom_amount**: Update a custom suggested donation amount
- **update_custom_field**: Update a custom field on donation forms
- **update_dedication_field**: Update a custom dedication field
- **update_dedication_type**: Update a dedication type
- **update_event**: Update a specific event
- **update_form_wording**: Update custom wording on organization forms
- **update_kiosk**: Update a specific kiosk
- **update_pledge**: Update a specific pledge
- **update_report_mapping**: Update a specific report mapping
- **update_restriction**: Update a specific restriction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qgiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our current organization and form-level settings."

**🤖 AI Agent:**
> I have retrieved your account settings using `get_account_settings`. Your organization is configured with standard receipting enabled, and default form-level settings are active. Would you like to update any of these settings?

---

**👤 You:**
> "List all the custom suggested donation amounts configured on our account."

**🤖 AI Agent:**
> I've fetched the custom suggested donation amounts using `list_custom_amounts`. You currently have four active tiers: $10, $25, $50, and $100. Would you like to modify any of these or create a new suggested amount?

---

**👤 You:**
> "Get the details for the custom field with ID 'cf_98765'."

**🤖 AI Agent:**
> Using `get_custom_field`, I retrieved the details for field 'cf_98765'. It is a text field labeled 'How did you hear about us?' and is currently set as optional on your main donation form.


## ❓ FAQ

**Q: How do I clone an existing donation form using the AI?**
You can use the `clone_form` tool. Provide the JSON payload containing the details of the form you wish to clone, and the agent will handle the cloning process for you.

**Q: Can I view and update the custom suggested donation amounts on my forms?**
Yes. You can list all custom suggested amounts using `list_custom_amounts`, retrieve a specific one with `get_custom_amount`, or update an existing amount using `update_custom_amount`.

**Q: How do I manage custom fields on my donation forms?**
You can list all custom fields using `list_custom_fields`, retrieve a specific field's details with `get_custom_field`, or create and update fields using `create_custom_field` and `update_custom_field`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qgiv](https://vinkius.com/mcp/qgiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qgiv** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qgiv` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qgiv** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qgiv": {
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
