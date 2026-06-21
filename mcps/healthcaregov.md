# HealthCare.gov MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/healthcaregov)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Automate marketplace research via HealthCare.gov — search for health plans, drugs, and providers directly from any AI agent.

## Description
Connect the **HealthCare.gov** Marketplace API to any AI agent and take full control of ACA health plan research and provider network verification through natural conversation.

### What you can do

- **Plan Search** — Retrieve available health and dental plans based on household demographics and location.
- **Drug Coverage** — Search for medications and verify if they are covered by specific plans and at what tier.
- **Provider Lookup** — Search for doctors, hospitals, and facilities and check their in-network status.
- **Geography Insights** — Retrieve County FIPS codes by ZIP code to ensure accurate regional pricing.
- **Issuer Details** — List all insurance companies operating in specific states and their available plans.
- **Crosswalk Access** — Monitor plan transitions between enrollment years to stay updated on coverage changes.

### How it works

1. Subscribe to this server
2. Enter your Marketplace API Key (from developer.cms.gov)
3. Start researching health plans from Claude, Cursor, or any MCP-compatible client

No more manual filtering through complex marketplace portals. Your AI assistant acts as a dedicated Health Insurance Navigator or Benefits Specialist.

### Who is this for?

- **Benefits Consultants** — instantly retrieve plan options and pricing for clients across different regions.
- **Healthcare Navigators** — automate the process of verifying provider networks and drug formularies.
- **Policy Researchers** — maintain a real-time overview of marketplace availability and issuer competition.


## Available Tools (11)
- **get_counties_by_zip**: Retrieve County FIPS codes for a given ZIP code
- **get_plan_crosswalk**: Get information about plan transitions between years
- **get_drug_coverage**: Check if a medication is covered by a specific plan
- **get_api_metadata**: Retrieve metadata about the Marketplace API data
- **get_plan_details**: Get detailed information about a specific health plan
- **get_provider_coverage**: Verify if a provider is in-network for a specific plan
- **list_issuers**: List insurance issuers operating in a specific state
- **list_market_states**: List states served by the Marketplace
- **search_drugs**: Search for medications in the Marketplace drug database
- **search_plans**: Pass household and place as JSON strings.

Search for health and dental plans in the Marketplace
- **search_providers**: Search for healthcare providers (doctors, facilities)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HealthCare.gov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for health plans in ZIP code 22102."

**🤖 AI Agent:**
> I've started the search for ZIP 22102. I first need to retrieve the County FIPS code for this area. It belongs to Fairfax County (FIPS: 51059). Should I now proceed to list available Silver plans for a 30-year-old individual?

---

**👤 You:**
> "Check if 'Lipitor' is covered by plan ID 12345VA001."

**🤖 AI Agent:**
> Checking drug coverage... I found 'Atorvastatin' (Generic Lipitor) in the database. For plan 12345VA001, it is covered as a Tier 1 (Generic) drug with a $10 copay. Would you like to check any other medications?

---

**👤 You:**
> "List all insurance companies operating in Virginia."

**🤖 AI Agent:**
> Accessing issuer data... In Virginia (VA), there are 8 main issuers operating in the Marketplace, including 'Anthem Health', 'CareFirst BlueCross BlueShield', and 'Kaiser Permanente'. Would you like to see the available plan counts for each?


## ❓ FAQ

**Q: How do I obtain a HealthCare.gov API Key?**
You must request a free API key through the **CMS Marketplace API** portal (developer.cms.gov/marketplace-api). Keys are typically sent via email and must be renewed every 60 days.

**Q: Can I check if my doctor is in-network for a specific plan?**
Yes! Use the `get_provider_coverage` tool by providing the plan ID and the provider ID. The agent will confirm the network status for that specific combination.

**Q: What geographic information is required for plan searches?**
Most searches require a 5-digit ZIP code and a 5-digit County FIPS code. You can use the `get_counties_by_zip` tool to retrieve the FIPS code for any ZIP code.

**Q: Is the integration secure for searching health data?**
Absolutely. The integration uses official CMS API keys over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/healthcaregov](https://vinkius.com/mcp/healthcaregov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HealthCare.gov** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `healthcaregov` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HealthCare.gov** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "healthcaregov": {
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
