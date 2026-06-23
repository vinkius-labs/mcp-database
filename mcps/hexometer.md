# Hexometer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hexometer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate website monitoring via Hexometer — monitor uptime, performance, and health directly from any AI agent.

## Description
Connect your **Hexometer** account to any AI agent and take full control of your website monitoring and technical health through natural conversation.

### What you can do

- **Performance Analysis** — Trigger on-demand page speed tests for desktop and mobile devices to ensure a fast user experience.
- **Asset Monitoring** — Identify heavy scripts, large images, and detected JavaScript errors affecting your site's health.
- **Site Oversight** — List all monitored properties and retrieve overall health scores and security statuses.
- **Availability Tracking** — Access historical uptime statistics and monitor recent alerts for service interruptions.
- **SEO Auditing** — Perform on-page SEO scans to analyze meta tags, headers, and broken link status.
- **Maintenance & Security** — Verify SSL certificate expiry and monitor general security posture across your digital assets.

### How it works

1. Subscribe to this server
2. Enter your Hexometer API Key (found in Property Settings > API)
3. Start monitoring your websites from Claude, Cursor, or any MCP-compatible client

No more manual checking of monitoring dashboards for performance updates. Your AI assistant acts as a dedicated Web Performance Engineer or Site Reliability Analyst.

### Who is this for?

- **Web Developers** — instantly retrieve JS error logs and page speed scores during development or staging.
- **SEO Specialists** — automate the auditing of meta tags and broken links for multiple properties.
- **E-commerce Owners** — monitor site uptime and performance trends to ensure consistent conversion rates.


## Available Tools (11)
- **check_broken_links**: List detected 404 errors and broken links for a property
- **check_page_errors**: Scan a page for JS errors and heavy assets
- **check_speed_desktop**: Returns scores and asset details.

Analyze desktop page speed for a specific URL
- **check_speed_mobile**: Analyze mobile page speed for a specific URL
- **get_site_health**: Get the overall health status for a specific property
- **get_security_status**: Retrieve SSL and general security health for a site
- **get_uptime_stats**: Get historical uptime statistics for a site
- **list_recent_alerts**: List recent monitoring alerts and notifications
- **list_monitored_sites**: List all websites (properties) tracked in Hexometer
- **list_wordpress_syncs**: List active WordPress plugin syncs
- **run_seo_audit**: Perform an on-demand SEO audit for a URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hexometer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the mobile page speed for 'https://example.com'."

**🤖 AI Agent:**
> Analyzing mobile performance... Example.com has a mobile speed score of 82/100. The largest contentful paint (LCP) is 2.4s. I also detected 3 heavy image assets that could be optimized. Would you like the full list of errors?

---

**👤 You:**
> "Show me the health status for property ID 'prop_123'."

**🤖 AI Agent:**
> Accessing site health... Property prop_123 is currently Healthy (Score: 94/100). Uptime is 100% for the last 30 days. However, the SSL certificate expires in 12 days. Should I set a reminder for the renewal?

---

**👤 You:**
> "Run an SEO audit for 'https://myblog.com/post-1'."

**🤖 AI Agent:**
> SEO audit complete! I've scanned the post. Meta titles and descriptions are well-optimized. However, 2 images are missing alt tags and there is no H1 header defined. Would you like me to suggest some improvements?


## ❓ FAQ

**Q: How do I find my Hexometer API Key?**
Log in to Hexometer, select a property from your dashboard, navigate to **Settings**, and you will find your unique **API Key** listed in the API section.

**Q: Can I trigger a performance check for any URL?**
Yes! The `check_speed_desktop`, `check_speed_mobile`, and `run_seo_audit` tools allow you to provide any URL. Hexometer will perform a real-time analysis and return the results.

**Q: Does the integration detect broken links?**
Yes, you can use the `check_broken_links` tool with a property ID to retrieve a list of all detected 404 errors and dead links identified by Hexometer's automated scans.

**Q: Is the integration secure for monitoring data?**
Absolutely. The integration uses official Hexometer API keys over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hexometer](https://vinkius.com/mcp/hexometer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hexometer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hexometer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hexometer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hexometer": {
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
