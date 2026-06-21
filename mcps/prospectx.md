# ProspectX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prospectx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Find and verify B2B prospect data with AI-powered enrichment that builds targeted outreach lists for your sales team.

## Description
Accelerate your real estate investing with an AI agent connected directly to ProspectX. Stop manually switching between lists and skip tracing tools—your agent can automatically find property owner contact info, filter distressed properties, and trigger targeted direct mail campaigns seamlessly.

### What you can do
- Filter and search for highly motivated seller leads
- Run instant skip tracing to discover owner phone numbers and emails
- Search properties by address, vacancy status, or type
- Manage and organize direct mail campaign lists
- Track the delivery and response rates of your marketing efforts

### How it works
1. Sign in to your ProspectX account
2. Navigate to Settings to generate your developer API key
3. Connect to Vinkius to enable AI-powered real estate prospecting

### Who is it for?
Designed for real estate investors, wholesalers, and acquisitions teams looking to automate their lead generation and outreach at scale.


## Available Tools
- **check_prospectx_status**: Verify connectivity
- **create_lead**: Create a lead
- **create_property_list**: Create a list
- **get_campaign**: Get campaign details
- **get_dashboard**: Get dashboard
- **get_lead**: Get lead details
- **get_property_list**: Get list details
- **get_property**: Get property details
- **list_campaigns**: List campaigns
- **list_leads_by_status**: Filter leads by status
- **list_leads**: List all leads
- **list_properties_by_type**: Filter properties by type
- **list_properties**: List properties
- **list_property_lists**: List property lists
- **search_properties**: Search properties
- **skip_trace**: Skip trace a property
- **update_lead**: Update a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProspectX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a skip trace on the property at 123 Main Street to find the owner's contact info"

**🤖 AI Agent:**
> Skip trace complete. The owner of 123 Main Street is John Doe. Primary phone: (555) 123-4567. Email: john@example.com.

---

**👤 You:**
> "Find all vacant properties in the database for a targeted mailing campaign"

**🤖 AI Agent:**
> I found 42 vacant properties matching your criteria. Would you like me to add them to your 'Q3 Direct Mail' campaign?

---

**👤 You:**
> "Show all hot leads that are ready for follow-up in ProspectX"

**🤖 AI Agent:**
> You have 5 hot leads ready for follow-up today. Sarah Connor requested a call back at 2 PM. Should I list the others?


## ❓ FAQ

**Q: What is skip tracing?**
Skip tracing finds the current phone number, email, and mailing address for property owners, enabling direct outreach to motivated sellers.

**Q: Can I search by property type?**
Yes, filter properties by type (residential, commercial, vacant, multi-family) to build targeted mailing lists for specific investment strategies.

**Q: How are campaigns tracked?**
View campaign status, delivery metrics, and response rates for all direct mail campaigns, with a centralized dashboard showing overall lead generation performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prospectx](https://vinkius.com/mcp/prospectx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProspectX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `prospectx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProspectX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prospectx": {
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
