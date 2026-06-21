# Candid (GuideStar) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/candid-guidestar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access comprehensive non-profit data via Candid — search organizations, verify charity status, and retrieve detailed financials directly from any AI agent.

## Description
Connect your **Candid (formerly GuideStar)** account to any AI agent and orchestrate your non-profit research, due diligence, and philanthropic data workflows through natural conversation.

### What you can do

- **Organization Oversight** — Search for non-profits by name, location, or NTEE code and retrieve basic metadata using the Essentials API.
- **Deep-Dive Profiles** — Access comprehensive data (Premier tier) including mission statements, leadership, and detailed financials.
- **Charity Compliance** — Verify IRS tax-exempt status and eligibility to receive tax-deductible contributions using the Charity Check tool.
- **Financial Auditing** — Retrieve detailed financial records and IRS Form 990 data straight from your workspace.
- **Demographics Analysis** — Access diversity, equity, and inclusion (DEI) data for organizations to inform your philanthropic strategy.
- **Organization Discovery** — Use the EIN (Employer Identification Number) as a primary key to fetch 760+ data fields for individual entities.

### How it works

1. Subscribe to this server
2. Enter your Candid API Subscription Key
3. Start exploring the non-profit sector from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Philanthropists & Foundations** — quickly verify charity statuses or retrieve financial health data without manual dashboard work.
- **Researchers & Analysts** — gather comprehensive non-profit metadata for reports straight from their workflow tools.
- **Developers** — integrate reliable non-profit data into their applications using natural language.


## Available Tools
- **get_charity_check_pdf**: Generate a PDF report for compliance record-keeping
- **get_demographics**: Get DEI data for a nonprofit
- **get_nonprofit_essentials**: Get core details for a nonprofit by EIN
- **get_grant_details**: Get specific details for a grant
- **get_nonprofit_eligibility**: Verify nonprofit eligibility for specific donation platforms
- **get_nonprofit_news**: Get real-time social sector news related to a nonprofit
- **get_nonprofit_premier**: Get comprehensive deep-dive data for a nonprofit by EIN
- **search_grants**: Search for grants awarded by foundations
- **search_nonprofits**: Search for nonprofits using filters
- **verify_charity_status**: Verify an organization's eligibility to receive tax-deductible contributions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Candid (GuideStar)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for non-profits in 'Miami' with the name 'Red Cross'."

**🤖 AI Agent:**
> I've found the results for 'Red Cross' in Miami. The primary entity is 'American Red Cross Greater Miami' (EIN: 59-0624xxx). Would you like to see their full profile?

---

**👤 You:**
> "Get detailed financial info for EIN 13-162xxxx."

**🤖 AI Agent:**
> Retrieving financial data for EIN 13-162xxxx... For the latest fiscal year, they reported total revenue of $5.2M, total expenses of $4.8M, and assets of $12M.

---

**👤 You:**
> "Verify the charity status for EIN 52-153xxxx."

**🤖 AI Agent:**
> EIN 52-153xxxx is currently listed as a 501(c)(3) public charity in good standing with the IRS. They are eligible to receive tax-deductible contributions.


## ❓ FAQ

**Q: Can I verify if a non-profit is eligible for tax-deductible donations?**
Yes! Use the `verify_charity_status` tool with the organization's EIN. Your agent will fetch the real-time compliance status from Candid's Charity Check API.

**Q: How do I find the EIN for an organization if I only have its name?**
Simply ask the agent to `search_nonprofits` and provide the name. The search results will include the EIN for each matching organization, which you can then use for deeper lookups.

**Q: Does the integration allow accessing diversity and inclusion data?**
Yes. Use the `get_demographics` tool. It will retrieve the DEI metadata provided by the organization to Candid, helping you understand their leadership and staff representation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/candid-guidestar](https://vinkius.com/mcp/candid-guidestar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Candid (GuideStar)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `candid-guidestar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Candid (GuideStar)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "candid-guidestar": {
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
