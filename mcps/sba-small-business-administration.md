# SBA (Small Business Administration) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sba-small-business-administration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Access official U.S. Small Business Administration data to check business size standards and retrieve geographic resource links.

## Description
Connect to the **U.S. Small Business Administration (SBA)** data services to verify business qualifications and access regional support resources through natural language.

### What you can do

- **Size Standard Verification** — Determine if a business qualifies as 'small' based on its NAICS code, annual revenue, or number of employees.
- **Geographic Resource Mapping** — Retrieve a comprehensive list of geographic links and resources provided by the SBA system.
- **Regional Filtering** — Access specific geographic links filtered by city or county to find local business support.
- **Regulatory Compliance** — Quickly check if a company meets federal size standards for government contracting or loan eligibility.

### How it works

1. Subscribe to this server
2. Access public SBA data endpoints directly through your AI agent
3. Start querying business statuses and geographic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Entrepreneurs & Small Business Owners** — quickly verify if your business meets SBA size standards for federal programs.
- **Government Contractors** — validate the small business status of potential partners or subcontractors using NAICS codes.
- **Financial Analysts** — automate the gathering of SBA geographic resources and business size data for reporting.


## Available Tools (3)
- **get_all_geographic_links**: Get all geographic links from the SBA system
- **get_city_county_links**: Get geographic links filtered by city or county
- **check_small_business_status**: Check if a business qualifies as small under SBA regulations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SBA (Small Business Administration)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a business with NAICS code 541511 and $15 million in revenue is considered small."

**🤖 AI Agent:**
> I've checked the SBA size standards for NAICS 541511 (Custom Computer Programming Services). Based on the $15 million revenue provided, the business qualifies as a small business under current SBA regulations.

---

**👤 You:**
> "Get all geographic links from the SBA system."

**🤖 AI Agent:**
> I have retrieved the comprehensive list of geographic links from the SBA. This includes regional office contacts, local resource partners, and state-specific business guides.

---

**👤 You:**
> "Find SBA city and county links for business support."

**🤖 AI Agent:**
> I've fetched the city and county specific links. You can now browse localized resources for small business development, including local counseling and financial assistance contacts.


## ❓ FAQ

**Q: How do I check if a business qualifies as a small business under SBA rules?**
Use the `check_small_business_status` tool. You will need to provide the 6-digit NAICS code for the industry, along with the average annual revenue or number of employees.

**Q: Can I find SBA resources for a specific city or county?**
Yes! Use the `get_city_county_links` tool to retrieve geographic links filtered by your target city or county.

**Q: What is the source of this data?**
The data is retrieved directly from the official U.S. Small Business Administration (SBA) public API endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sba-small-business-administration](https://vinkius.com/mcp/sba-small-business-administration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SBA (Small Business Administration)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sba-small-business-administration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SBA (Small Business Administration)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sba-small-business-administration": {
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
