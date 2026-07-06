# CUFinder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cufinder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Discover verified B2B contact data including emails, phone numbers, and company info for targeted sales prospecting.

## Description
Connect your **CUFinder** business intelligence account to any AI agent and simplify how you discover professional domains, enrich company metadata, and identify decision makers through natural conversation.

### What you can do

- **Domain Discovery** — Find the primary web domain for any company using only its trade name via AI.
- **Company Intelligence** — Retrieve detailed metadata including industry, location, and estimated annual revenue for specific domains.
- **Employee Prospecting** — List known employees and key decision makers associated with a company domain.
- **LinkedIn Enrichment** — Fetch detailed contact info and professional data from specific LinkedIn profile URLs.
- **Lead Qualification** — Verify company size and financial standing to prioritize your sales outreach.
- **Data Accuracy** — Enhance your CRM records with verified real-time data directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your CUFinder API Key (found in your account dashboard)
3. Start enriching your sales pipeline from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & SDR Teams** — quickly find company domains and decision maker lists via simple AI commands.
- **Marketing & Growth** — enrich lead lists with revenue and industry data directly from the workspace.
- **Business Analysts** — perform quick competitive intelligence and market research via the AI assistant.


## Available Tools (13)
- **find_employees**: Find employees
- **find_phone**: Find phone number
- **get_account**: Get account info
- **get_company_info**: Get company info
- **get_company_socials**: Get social profiles
- **get_company_tech**: Get tech stack
- **get_company_revenue**: Get company revenue
- **enrich_linkedin**: Enrich LinkedIn profile
- **verify_email**: Verify email
- **bulk_enrich**: Bulk enrich
- **check_cufinder_status**: Verify connectivity
- **find_domain**: Find company domain
- **find_email**: Find email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CUFinder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the domain for the company 'Acme Global Solutions'."

**🤖 AI Agent:**
> I've found the domain. The primary website for 'Acme Global Solutions' is acme-global.com. Would you like me to retrieve the company's full metadata and revenue estimate?

---

**👤 You:**
> "Show me the employees and decision makers for 'apple.com'."

**🤖 AI Agent:**
> Fetching employee data... I've identified several key contacts for apple.com, including roles in 'Product Management', 'Engineering', and 'Marketing'. Would you like the contact details for any of them?

---

**👤 You:**
> "Enrich the data from this LinkedIn URL: 'https://linkedin.com/in/stevejobs'."

**🤖 AI Agent:**
> Enrichment complete! For the provided profile, I've retrieved full metadata including professional title, current company (Apple), and verified contact information. I've updated the profile record with these insights.


## ❓ FAQ

**Q: Can I find the official website for a company via AI?**
Yes! Use the `find_company_domain` tool and provide the company name. Your agent will return the primary web domain registered for that entity.

**Q: How do I see the estimated revenue for a specific company?**
Run the `get_company_revenue` query and provide the domain. The agent will retrieve the estimated annual revenue range from CUFinder's database.

**Q: Is it possible to list employees for a domain via AI?**
Absolutely. Use the `find_company_employees` tool. The agent will retrieve a list of known employees and decision makers associated with that specific company domain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cufinder](https://vinkius.com/mcp/cufinder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CUFinder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cufinder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CUFinder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cufinder": {
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
