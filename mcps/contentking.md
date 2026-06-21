# ContentKing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Enable your AI agent to fetch real-time SEO audit metrics and monitor website changes through ContentKing.

## Description
Integrate your AI with **ContentKing**, the real-time SEO auditing and monitoring platform.

### What you can do

- **Site Audits** — Review crawled pages and identify active SEO risks or technical errors instantly.
- **Change Monitoring** — Get summaries of recent alerts or infrastructure changes impacting SEO.
- **Metric Retrieval** — Fetch health scores and page-level data for your reporting workflows.

### How it works

1. Add the ContentKing integration to your AI toolset.
2. Supply your ContentKing API Key.
3. Query domains and site metrics via natural language commands.

### Who is this for?

- **SEO Specialists** — Diagnose organic performance without manual dashboard reviews.
- **Web Developers** — Audit post-deployment changes to validate infrastructure health.
- **Digital Marketers** — Pull comparative domain health data quickly.


## Available Tools
- **get_active_alerts**: Get active monitoring alerts for a website
- **get_issue_details**: Get details for a specific SEO issue
- **get_portfolio_summary**: Get a high-level health summary across all websites
- **get_website_health**: Get current health score and status for a website
- **list_seo_issues**: List SEO issues for a website
- **list_monitored_pages**: List monitoring data for pages on a website
- **list_websites**: List all websites monitored in ContentKing
- **notify_page_update**: Notify ContentKing of page updates to trigger re-crawl
- **notify_sitemap_update**: Notify ContentKing that a sitemap has been updated
- **search_pages_by_url**: Search for monitored pages by URL keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ContentKing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current health score for 'vinkius.com'."

**🤖 AI Agent:**
> The domain 'vinkius.com' has a health score of 94/100. The latest crawl finished 2 minutes ago. Would you like a breakdown of the remaining issues?

---

**👤 You:**
> "List all critical alerts for meta tag changes today."

**🤖 AI Agent:**
> 2 critical alerts today related to meta tags:
1. The 'Title' tag was removed from the homepage — severe warning.
2. A canonical tag created a self-referencing loop on '/products/sales'.
Both require developer attention.

---

**👤 You:**
> "Give me a high-level summary of the health of all my monitored websites."

**🤖 AI Agent:**
> I've analyzed your portfolio. You have 5 websites with an average health score of 88/100. 3 sites are in excellent health, while 'dev-blog.com' shows a recent dip to 64/100 due to new accessibility issues. Would you like to see the details for that site?


## ❓ FAQ

**Q: How do I get a ContentKing API Key?**
Log in to ContentKing, go to **Account Settings > API**, and click **Create API Key**. Copy the key and paste it into the field below.

**Q: Can the agent make changes to my SEO settings?**
No. The integration operates in read-only mode. It reads metrics, lists alerts, and retrieves data for analysis, but cannot modify any SEO settings or configurations.

**Q: What types of metrics can I check?**
You can fetch domain health scores, tracked URL counts, active alerts by severity, page load times, and summaries of issues found during the latest crawls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentking](https://vinkius.com/mcp/contentking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ContentKing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `contentking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ContentKing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contentking": {
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
