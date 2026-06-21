# DealMachine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dealmachine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Equip your AI agent to manage real estate leads, track properties, and monitor marketing campaigns via the DealMachine API.

## Description
Integrate **DealMachine**, the leading CRM for real estate investors, directly into your AI workflow. Manage your real estate leads, research property ownership and equity data, and monitor direct mail marketing campaigns using natural language.

### What you can do

- **Lead Management** — List, search, and retrieve detailed profiles for your real estate leads.
- **Property Research** — Access full data for tracked properties including owner names, equity, and mortgage information.
- **Campaign Oversight** — Monitor active direct mail and marketing campaigns directly via chat.
- **Team Coordination** — List driving teams and members associated with your account.

### How it works

1. Connect the DealMachine integration to your AI assistant.
2. Authorize using your DealMachine API Key (found in your account settings).
3. Accelerate your real estate investing through intuitive conversation.

### Who is this for?

- **Real Estate Investors** — Quickly check lead details and property equity on the go.
- **Wholesalers** — Research property ownership and manage new leads during field research.
- **Real Estate Teams** — Monitor marketing campaigns and coordinate team activities via chat.


## Available Tools (10)
- **add_new_lead**: Persists a new lead based on property address, initiating property data resolution and owner identification.

Add a new real estate lead to your CRM
- **get_account_details**: Returns account-level metadata including subscription plan, credit balance, and organizational settings.

Retrieve metadata and plan limits for your DealMachine account
- **get_lead_details**: Resolves associated property details, owner contact information, and the history of marketing actions taken.

Get detailed information for a specific real estate lead
- **get_property_details**: Resolves technical data such as estimated equity, mortgage information, deed history, and detailed owner metadata.

Get full data for a specific property including owner and equity
- **list_marketing_campaigns**: Returns campaign summaries including send dates, recipient counts, and engagement metrics.

List all direct mail and marketing campaigns
- **list_real_estate_leads**: Returns lead metadata including property addresses, owner names, and current lead status (e.g., potential, contacted).

List all real estate leads in your DealMachine account
- **list_tracked_properties**: Returns address data and internal property identifiers.

List all properties tracked in the system
- **list_lead_tags**: Returns tag names and identifiers used for filtering leads and properties.

List all tags used to categorize leads and properties
- **list_driving_teams**: Returns a list of teams, active drivers, and their respective roles within the DealMachine workspace.

List all teams and members associated with your account
- **search_leads_by_address**: Matches the search term against property addresses and owner names using partial case-insensitive matching.

Search for leads by address or owner name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DealMachine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent real estate leads."

**🤖 AI Agent:**
> I've found 5 recent leads, including '123 Maple St' and '456 Oak Ave'. Would you like to see the ownership details for '123 Maple St'?

---

**👤 You:**
> "Show me the details for property '123 Maple St'."

**🤖 AI Agent:**
> Property '123 Maple St' is owned by 'John Doe'. It has an estimated equity of 65% and no active mortgage reported in public records. Should I check if they are part of any marketing campaign?

---

**👤 You:**
> "What marketing campaigns are currently running?"

**🤖 AI Agent:**
> You have 2 active direct mail campaigns: 'Probate List June' and 'High Equity - South Side'. A total of 1,200 postcards were sent this week. Would you like a list of leads that responded?


## ❓ FAQ

**Q: How do I get a DealMachine API Key?**
Log in to your DealMachine account, navigate to **Settings > API**, and you can generate or retrieve your API Key from that section.

**Q: Can the agent create new leads?**
Yes, you can use the add_new_lead tool to add a property address directly to your DealMachine CRM via the agent.

**Q: Does the integration show property equity?**
Yes, when retrieving property details, the agent can provide information on owner equity and other public records data available in your plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dealmachine](https://vinkius.com/mcp/dealmachine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DealMachine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dealmachine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DealMachine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dealmachine": {
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
