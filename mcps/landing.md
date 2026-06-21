# Landing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/landing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create high-converting landing pages in minutes with AI-powered templates and drag-and-drop editing built for marketers.

## Description
Connect your **Landing** account to any AI agent and manage landing pages through natural conversation.

### What you can do

- **Page Management** — List, create, and manage landing pages
- **Lead Tracking** — Browse captured leads with form data and conversion source
- **Template Library** — Access pre-built templates for quick page creation
- **Analytics Monitoring** — Track page views, conversions, and bounce rates

### How it works

1. Subscribe to this server
2. Enter your Landing Access Token
3. Start managing pages from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing** — manage campaigns and landing pages
- **Growth** — track conversion rates and leads
- **Designers** — access templates and page configurations


## Available Tools
- **create_landing_webhook**: g., lead.created).

Create a new webhook
- **delete_landing_webhook**: Delete a webhook
- **get_my_landing_profile**: Get authenticated user info
- **list_landing_leads**: List captured leads
- **list_landing_pages**: List landing pages
- **list_landing_projects**: List all landing projects
- **list_landing_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Landing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all landing pages with conversion rates and today's leads."

**🤖 AI Agent:**
> Pages: 6 active. 'SaaS Free Trial' (4.2K views, 8.5% conversion ⭐). 'Webinar Registration' (2.1K, 12.3%). 'Product Demo' (1.8K, 6.1%). 'E-book Download' (3.4K, 15.2% ⭐). 'Pricing Page' (5.1K, 3.8%). 'Contact Us' (890, 22.4%). Today's leads: 18. Top: 'E-book' (7), 'Webinar' (5), 'SaaS' (4).

---

**👤 You:**
> "Show leads captured from the SaaS Free Trial page this week."

**🤖 AI Agent:**
> SaaS Free Trial leads (7 days): 32. By source: Google Ads (14, 44%), Organic (8, 25%), LinkedIn (6, 19%), Direct (4, 12%). Top: 1) john@acmecorp.com — CTO, 50+ employees. 2) sarah@techco.com — VP Eng, 200+. 3) mike@startup.io — Founder, 10-50. Conversion rate: 8.5%. Cost per lead (paid): $12.40.

---

**👤 You:**
> "Browse templates and show page analytics for the Webinar page."

**🤖 AI Agent:**
> Templates: 15 available. Categories: SaaS (4), E-commerce (3), Education (2), Agency (3), Event (3). Webinar analytics: Views: 2.1K (7 days). Unique visitors: 1.8K. Conversion: 12.3% (258 registrations). Bounce rate: 38%. Avg time on page: 1.8 min. Traffic: Organic 40%, Paid 35%, Social 25%.


## ❓ FAQ

**Q: Can I track leads and conversion rates?**
Yes. Browse all captured leads with form data, traffic source, and timestamp. Monitor conversion rates per page.

**Q: Can I manage and create landing pages?**
Yes. List all pages with status, create new pages, and manage page settings and publication status.

**Q: What API does Landing use?**
Bearer authentication against `api.landing.com/v1`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/landing](https://vinkius.com/mcp/landing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Landing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `landing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Landing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "landing": {
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
