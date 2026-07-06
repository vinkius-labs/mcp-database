# Google Search Console MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-search-console)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor your website's search performance, fix indexing issues, and manage sitemaps via AI.

## Description
Connect your **Google Search Console** to your AI agent and take control of your technical SEO. Use natural language to query search traffic data, inspect URLs for indexing errors, and manage your sitemaps across all your verified web properties.

### What you can do

- **Search Analytics** — Query clicks, impressions, CTR, and position data by date, country, device, or specific queries
- **URL Inspection** — Instantly check if a specific page on your site is indexed by Google and identify any mobile usability or indexing errors
- **Sitemap Management** — List all submitted sitemaps, verify their status, and submit new ones directly from the chat
- **Site Management** — View all your verified properties and add or remove sites from your Search Console account

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Client ID and Secret
3. Complete the secure Google authorization flow
4. Start analyzing your SEO performance from Claude, Cursor, or any MCP-compatible client

Stop wrestling with the Search Console UI. Your AI agent acts as your dedicated technical SEO analyst.

### Who is this for?

- **SEO Specialists** — quickly pull search query data for specific landing pages or verify if a recently launched page has been indexed
- **Web Developers** — automate URL inspections during deployments and ensure sitemaps are processed correctly
- **Content Marketers** — find out what keywords are driving traffic to your blog posts through simple conversational queries


## Available Tools (10)
- **list_sitemaps**: List submitted sitemaps for a site
- **list_sites**: List verified sites in Search Console
- **query_search_analytics**: Query search traffic data
- **submit_sitemap**: Submit a new sitemap
- **add_site**: Add a site to Search Console
- **delete_site**: Remove a site from Search Console
- **delete_sitemap**: Delete a submitted sitemap
- **get_site**: Get details for a specific site
- **get_sitemap**: Get details about a specific sitemap
- **inspect_url**: Inspect the index status of a specific URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Search Console** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if https://mysite.com/new-post is indexed by Google."

**🤖 AI Agent:**
> Inspecting URL... The URL is successfully indexed and can appear in Google Search results. Mobile usability is marked as 'Pass'.

---

**👤 You:**
> "What were the top 5 search queries for our site last week?"

**🤖 AI Agent:**
> Querying search analytics... Here are your top 5 queries from the last 7 days:
1. 'buy coffee beans online' (450 clicks, 1200 impressions)
2. 'best dark roast' (320 clicks, 900 impressions)
3. 'organic espresso' (210 clicks, 800 impressions)
4. 'fair trade coffee' (150 clicks, 600 impressions)
5. 'coffee subscription box' (90 clicks, 400 impressions)

---

**👤 You:**
> "Submit our new sitemap at https://mysite.com/sitemap-products.xml to Search Console."

**🤖 AI Agent:**
> Sitemap successfully submitted to Google Search Console.
**Status**: Pending processing by Googlebot. We will monitor its progress actively.


## ❓ FAQ

**Q: Can I check why a specific page isn't appearing in Google?**
Yes. Use the `inspect_url` tool to run a live inspection on the URL. The AI will return the index status and highlight any errors, such as 'Noindex detected' or mobile usability issues.

**Q: How do I find out my top performing keywords?**
You can ask the AI to `query_search_analytics` with the dimension set to 'query'. It will return your top keywords based on clicks and impressions for the requested date range.

**Q: Can I submit a new XML sitemap through this integration?**
Absolutely! Use the `submit_sitemap` tool, provide your site URL and the path to your sitemap (e.g., 'https://example.com/sitemap.xml'). Google will schedule it for processing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-search-console](https://vinkius.com/mcp/google-search-console)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Search Console** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-search-console` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Search Console** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-search-console": {
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
