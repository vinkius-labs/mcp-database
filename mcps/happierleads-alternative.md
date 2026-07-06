# HappierLeads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/happierleads-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Identify the companies visiting your website and match them to decision-makers for warm outbound prospecting that converts.

## Description
Connect your **HappierLeads** account to any AI agent and turn anonymous website traffic into identified B2B leads through natural conversation.

### What you can do

- **Visitor Identification** — List all identified B2B visitors with company data, filter by country, and search by company name or domain
- **Lead Management** — Browse all identified companies, filter by industry vertical, and focus on qualified high-intent leads
- **Session Analysis** — Inspect individual browsing sessions with page-by-page navigation paths and time spent
- **Page View Tracking** — List all pages viewed by a specific visitor for engagement insights
- **Segmentation** — Browse saved visitor segments and inspect criteria for targeted analysis
- **Real-Time Alerts** — Access notifications for high-value visitor activity
- **Analytics Dashboard** — Retrieve traffic overview: visitor count, identified companies, conversion rates, and top pages

### How it works

1. Subscribe to this server
2. Enter your HappierLeads API Key from your account settings
3. Start identifying leads from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — identify which companies visit your website and prioritize outreach based on browsing behavior
- **Marketing Teams** — analyze traffic sources, segment visitors, and track campaign-driven visits
- **Growth Teams** — monitor high-intent pages like pricing and demo requests to identify warm leads


## Available Tools (17)
- **get_session**: Get session details
- **get_visitor**: Get visitor details
- **list_leads_by_industry**: Filter leads by industry
- **list_leads**: List identified leads
- **list_notifications**: List notifications
- **list_page_views**: List page views
- **list_qualified_leads**: List qualified leads
- **list_segments**: List segments
- **list_sessions**: List visitor sessions
- **list_visitors_by_country**: Filter visitors by country
- **list_visitors**: List website visitors
- **search_visitors**: Search visitors
- **check_happier_status**: Verify connectivity
- **get_analytics**: Get analytics overview
- **get_lead**: Get lead details
- **get_segment**: Get segment details
- **get_top_pages**: Get top pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HappierLeads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all qualified leads from this week and the pages they viewed."

**🤖 AI Agent:**
> 8 qualified leads this week. Top 3 by engagement: 1) 'Acme Technologies' (SaaS, 250 employees) — 4 sessions, viewed /pricing (3 min), /enterprise (2 min), /demo (1 min). Strong buying signal. 2) 'DataFlow Corp' (Data Analytics, 120 employees) — 3 sessions, viewed /integrations (4 min), /api-docs (6 min), /pricing (2 min). Technical evaluation in progress. 3) 'GreenLogix' (Logistics, 500 employees) — 2 sessions, viewed /case-studies (5 min), /contact (30s). Research phase. Would you like to see their full session paths or filter by industry?

---

**👤 You:**
> "Show the analytics dashboard and which pages drive the most identified companies."

**🤖 AI Agent:**
> Analytics overview (last 30 days): Total visitors: 12,400. Identified companies: 342 (2.8% identification rate). Qualified leads: 89. Returning visitors: 156. Top pages by identified company visits: 1) /pricing — 78 companies (22.8%). 2) /features — 65 companies (19%). 3) /blog/ai-tools — 52 companies (15.2%). 4) /case-studies — 44 companies (12.9%). 5) /integrations — 38 companies (11.1%). High-intent signal: 23 companies visited both /pricing and /demo this month. Would you like to see the segments or check real-time notifications?

---

**👤 You:**
> "Search for visitors from 'fintech' companies and show sessions for the most engaged one."

**🤖 AI Agent:**
> Found 12 fintech visitors this month. Most engaged: 'PayStream Technologies' (visitor_891, fintech, 180 employees, London). 6 sessions over 3 weeks. Session breakdown: Session 1 (Apr 5): /home → /features → /pricing (8 min total). Session 2 (Apr 9): /blog/payment-apis → /integrations (12 min). Session 3 (Apr 14): /pricing → /enterprise → /security (15 min). Session 4 (Apr 18): /case-studies/fintech → /demo (6 min). Session 5 (Apr 22): /api-docs → /developer (18 min). Session 6 (Apr 25): /contact (2 min). This shows a classic evaluation journey — from research to technical review to contact. High priority for outreach!


## ❓ FAQ

**Q: Can I identify which companies are visiting my website?**
Yes! The `list_visitors` tool retrieves all identified B2B website visitors with company name, industry, employee count, and visit details. Use `search_visitors` to find specific companies by name or domain, and `list_visitors_by_country` to filter by geographic region. Use `get_visitor` for the full company profile.

**Q: Can I see which pages each company visited and how long they stayed?**
Yes. Use `list_sessions` with a Visitor ID to see all browsing sessions, then `get_session` for page-by-page navigation paths with time spent per page. Use `list_page_views` to get all pages viewed by a specific visitor. This reveals purchase intent — visitors spending time on pricing or demo pages are warm leads.

**Q: Can I focus only on high-intent qualified leads?**
Yes. The `list_qualified_leads` tool retrieves only leads that meet your qualification criteria (e.g., multiple visits, pricing page views, minimum session duration). Use `list_leads_by_industry` to further filter by vertical. Use `list_notifications` for real-time alerts when high-value visitors are on your site.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/happierleads-alternative](https://vinkius.com/mcp/happierleads-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HappierLeads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `happierleads-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HappierLeads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "happierleads-alternative": {
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
