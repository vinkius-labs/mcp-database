# Foxentry MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foxentry)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate and autocomplete addresses, emails, and phone numbers in forms to eliminate bad data before it enters your systems.

## Description
Connect your **Foxentry** data intelligence account to any AI agent and simplify how you clean your contact lists, verify identity data, and lookup business registrations through natural conversation.

### What you can do

- **Email Validation** — Instantly check if an email address is valid, active, and safe for your outreach campaigns.
- **Phone Intelligence** — Verify phone numbers and formats globally to ensure your communication reaches the right recipient.
- **Address Autocomplete** — Validate physical addresses and retrieve structured geographic metadata and zip codes via AI.
- **Business Lookup** — Fetch official company data, including registration names and registered addresses, using ID numbers.
- **Name Analysis** — Verify person names and automatically identify gender and name components (first, last, degree).
- **Data Accuracy** — Enhance your CRM records with verified real-time data directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Foxentry API Key (found in your account settings)
3. Start validating your audience data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & Marketing Teams** — quickly verify lead data and clean contact lists via simple AI commands.
- **Finance & Admin Staff** — lookup company registration details and verify billing addresses directly from the workspace.
- **Developers** — test data validation logic and verify API responses via the AI assistant.


## Available Tools (12)
- **check_foxentry_status**: Verify connectivity
- **format_phone**: Format phone
- **geocode_address**: Geocode address
- **get_business_details**: Get business details
- **lookup_business**: Lookup business
- **suggest_address**: Suggest address
- **suggest_email**: Suggest email
- **suggest_name**: Suggest name
- **validate_address**: Validate address
- **validate_email**: Validate email
- **validate_name**: Validate name
- **validate_phone**: Validate phone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foxentry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the email 'john.doe@example.com'."

**🤖 AI Agent:**
> Verification complete! The email 'john.doe@example.com' is marked as 'Valid' and active. No disposable domains or catch-all issues were detected. It is safe for your campaign.

---

**👤 You:**
> "Lookup business data for registration number '12345678' in Czech Republic."

**🤖 AI Agent:**
> I've found the record. The registration number belongs to 'Acme Tech s.r.o.' located in Prague. Their primary business industry is 'Software Development'. Would you like the full address?

---

**👤 You:**
> "Check if the phone number '+420 777 123 456' is valid."

**🤖 AI Agent:**
> Fetching phone data... The number +420 777 123 456 is 'Valid' and formatted correctly for the Czech Republic. It is identified as a mobile device.


## ❓ FAQ

**Q: Can I verify if a physical address is valid via AI?**
Yes! Use the `validate_physical_address` tool and provide the address string. Your agent will return the structured, autocompleted data and verification status.

**Q: How do I check if an email address is active using the agent?**
Use the `validate_email` tool. Provide the address, and Foxentry will check for syntax, domain validity, and if the specific mailbox actually exists.

**Q: Is it possible to retrieve business data using a registration number via AI?**
Absolutely. Use the `lookup_business_data` query and provide the registration number. The agent will retrieve official company names and registered addresses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foxentry](https://vinkius.com/mcp/foxentry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foxentry** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foxentry` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foxentry** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foxentry": {
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
