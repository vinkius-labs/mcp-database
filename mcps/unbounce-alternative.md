# Unbounce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unbounce-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Build high-converting landing pages with AI-powered optimization that tests headlines, copies, and layouts automatically.

## Description
Connect your **Unbounce** account to any AI agent and simplify how you manage your conversion-focused landing pages, lead data, and custom domains through natural conversation.

### What you can do

- **Landing Page Control** — List and inspect all landing pages across your sub-accounts and retrieve detailed configuration metadata.
- **Lead Analysis** — List and query all leads submitted through your forms, and retrieve individual lead data for processing.
- **Domain Oversight** — List custom domains registered in your account to verify connectivity and SSL status.
- **Account Organization** — Manage sub-accounts and page groups to keep your marketing assets structured.
- **Form Insight** — List all form fields across page variants to understand your data collection points.
- **User Monitoring** — Fetch account details and verify your current Unbounce user profile.

### How it works

1. Subscribe to this server
2. Enter your Unbounce API Key (found in your account API management)
3. Start managing your landing pages from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly check page performance and retrieve new leads via simple AI queries.
- **Web Developers** — verify domain configurations and form field structures directly from the workspace.
- **Conversion Optimizers** — get instant bird's-eye views of page groups and variant data via the AI assistant.


## Available Tools
- **list_accounts**: List all Unbounce accounts
- **list_domains**: List custom domains
- **list_form_fields**: List form fields for a page
- **get_lead**: Get details for a specific lead
- **get_page**: Get details for a specific landing page
- **list_leads**: List leads for a page
- **get_me**: Get current Unbounce user details
- **list_page_groups**: List page groups
- **list_pages**: List pages for a sub-account
- **list_sub_accounts**: List sub-accounts (clients)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unbounce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all landing pages in my sub-account '10293'."

**🤖 AI Agent:**
> I've retrieved your pages. You have 3 active landing pages: 'Summer Promo', 'E-book Download', and 'Product Beta Waitlist'. Which one would you like to see leads for?

---

**👤 You:**
> "Show me the latest 5 leads from the 'Summer Promo' page."

**🤖 AI Agent:**
> I've fetched the latest leads. There are 5 recent submissions including 'John Doe' (john@example.com) and 'Sarah Smith'. Shall I retrieve the full profile details for any of them?

---

**👤 You:**
> "Check the status of custom domains in my account."

**🤖 AI Agent:**
> Fetching domains... You have 2 registered domains: 'promo.vinkius.com' (Ready/SSL Active) and 'offers.vinkius.com' (CNAME pending). Would you like instructions on how to finish the setup?


## ❓ FAQ

**Q: Can I see all the leads collected by a specific landing page?**
Yes! Use the `list_leads` tool and provide the Page ID. Your agent will retrieve the complete list of submissions for that page.

**Q: How do I list all landing pages in a sub-account?**
Use the `list_pages` query with your Sub-Account ID. The agent will return all landing pages associated with that specific client or project area.

**Q: Is it possible to see the form fields used on a page via AI?**
Absolutely. Run the `list_form_fields` query with your Page ID. The agent will retrieve all form fields defined across all variants of that landing page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unbounce-alternative](https://vinkius.com/mcp/unbounce-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unbounce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unbounce-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unbounce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unbounce-alternative": {
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
