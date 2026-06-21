# LinkedIn Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-ads-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with direct access to LinkedIn Ads — manage campaigns, track B2B ad performance, and optimize LinkedIn marketing spend without opening Campaign Manager.

## Description
Connect **LinkedIn Ads** to your AI agent and manage your B2B advertising campaigns conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, campaign groups, and creatives.
- **B2B Analytics** — Pull impressions, clicks, CTR, CPC, leads, and cost-per-lead metrics.
- **Audience Targeting** — Query targeting by job title, company, industry, seniority, and matched audiences.
- **Lead Gen Forms** — Access lead gen form submissions and sync leads to your CRM.

### How it works

1. Subscribe to the LinkedIn Ads integration on the marketplace.
2. Create an app in the LinkedIn Developer Portal (developer.linkedin.com → My Apps → Create App).
3. Ask your AI agent to manage campaigns, pull reports, or download leads.

### Who is this for?

- **B2B Marketers** — Monitor and optimize LinkedIn ad spend targeting professionals and decision-makers.
- **Demand Gen Teams** — Track lead gen form submissions and campaign ROI conversationally.
- **Agencies** — Manage multiple client LinkedIn advertising accounts from one interface.


## Available Tools
- **list_campaign_groups**: List campaign groups
- **list_campaigns**: List campaigns
- **list_creatives**: List ad creatives
- **get_campaign_analytics**: Get campaign analytics
- **get_account_info**: Get ad account info
- **pause_campaign**: Pause campaign
- **enable_campaign**: Enable campaign
- **get_account_analytics**: Get account analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How are my LinkedIn campaigns performing this month?"

**🤖 AI Agent:**
> This month: Total spend: $8,200. Impressions: 340K. Clicks: 2,100. CTR: 0.62%. CPC: $3.90. Leads: 145. CPL: $56.55. Top campaign: 'VP Sales Targeting' (42 leads, $48 CPL).

---

**👤 You:**
> "Download all leads from my 'CTO Retargeting' campaign."

**🤖 AI Agent:**
> Downloaded 67 leads from 'CTO Retargeting'. Fields: name, email, company, job title, company size. 89% have valid business emails. Ready for CRM sync.

---

**👤 You:**
> "Increase the daily budget on 'Brand Awareness' campaign to $200."

**🤖 AI Agent:**
> Budget updated: 'Brand Awareness' daily budget changed from $150 to $200 (+33%). Estimated new daily reach: ~2,800 impressions (up from ~2,100).


## ❓ FAQ

**Q: How do I get my LinkedIn Ads API credentials?**
1. Go to **developer.linkedin.com** and log in with your LinkedIn account.
2. Click **My Apps** → **Create App**.
3. Fill in your app name, company LinkedIn page, and logo.
4. Under the **Products** tab, request access to **Marketing Developer Platform**.
5. After approval, go to the **Auth** tab and copy your **Client ID** and **Client Secret**.
6. Paste both values below.

⚠️ Access to the Marketing API requires approval from LinkedIn (typically 1-5 business days).

**Q: Can I download lead gen form submissions?**
Yes. Your AI agent can pull all lead gen form submissions including names, emails, job titles, and custom fields — ready to sync to your CRM or outreach tool.

**Q: What targeting criteria can I use?**
LinkedIn offers the most precise B2B targeting: job title, job function, seniority, company name, company size, industry, skills, education, and matched audiences (ABM lists, retargeting, lookalikes).

**Q: Can I track cost-per-lead (CPL)?**
Yes. Your AI agent calculates CPL by dividing total spend by leads generated — broken down by campaign, ad group, or creative. Essential for B2B marketers optimizing demand gen budgets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-ads-1](https://vinkius.com/mcp/linkedin-ads-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `linkedin-ads-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-ads-1": {
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
