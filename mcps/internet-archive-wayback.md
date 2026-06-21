# Internet Archive Wayback MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive-wayback)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Check URL archival status, explore capture history, and analyze Wayback Machine data.

## Description
Connect the **Internet Archive Wayback Machine** to any AI agent and access the world's largest web archive — 800B+ archived web pages spanning 25+ years of internet history.

### What you can do
- **URL Availability Check** — Verify if any URL has been archived and find the latest snapshot
- **Full CDX Capture History** — Get detailed capture history with timestamps, status codes, MIME types, and sizes
- **Filter by Year** — Find all captures from a specific year for temporal analysis
- **Filter by HTTP Status** — Find captures that returned specific status codes (200, 404, 301, 500)
- **Filter by MIME Type** — Find captures of specific resource types (HTML, images, PDFs, CSS)
- **First Capture** — Find when a URL was first archived
- **Latest Capture** — Find the most recent archived version of a URL
- **Capture Count** — Get the total number of times a URL has been archived
- **Deduplicated Captures** — Get unique captures collapsed by URL key
- **Subdomain Discovery** — Find all archived subdomains of a domain

### How it works
1. Subscribe to this server
2. No API key needed — completely free and public
3. Start exploring web history from Claude, Cursor, or any MCP-compatible client

The Wayback Machine is a non-profit service preserving internet history — no authentication required for access.

### Who is this for?
- **Journalists & Researchers** — find archived versions of websites to verify claims, track content changes, and recover deleted information
- **Web Developers** — analyze how websites evolved over time, compare design changes, and find historical implementations
- **Legal & Compliance** — preserve evidence of website content at specific points in time for legal proceedings
- **Historians & Academics** — study the evolution of the internet, track how organizations presented themselves online over decades
- **Cybersecurity** — investigate phishing sites, track domain changes, and discover subdomain footprints


## Available Tools (10)
- **get_captures_by_mime_type**: Common types: "text/html" (web pages), "image/jpeg" (JPEG images), "application/pdf" (PDFs), "text/css" (stylesheets). Use this to find specific resource types in the archive.

Get captures filtered by MIME type
- **get_captures_by_status**: Common codes: "200" (OK), "404" (Not Found), "301" (Redirect), "500" (Server Error). Use this to analyze site availability patterns over time.

Get captures filtered by HTTP status code
- **get_captures_by_year**: Use this to analyze archival frequency or find snapshots from a particular year. Year should be 4-digit format (e.g., "2020").

Get captures filtered by a specific year
- **get_cdx_captures**: Each capture includes timestamp, original URL, MIME type, HTTP status code, and file size. Use this for comprehensive archival analysis. Optional limit parameter controls maximum results.

Get detailed capture history from the CDX server
- **check_availability**: Returns the closest (most recent) snapshot timestamp and availability status. Use this to verify if a page is preserved and find its latest archived version.

Check if a URL has been archived by the Wayback Machine
- **get_captures_collapsed**: This shows unique page captures without redundant entries for the same page. Use this for a cleaner view of archived content.

Get captures deduplicated by URL key
- **get_capture_count**: Use this to measure how frequently a page has been preserved over time.

Get the total number of captures for a URL
- **get_first_capture**: Includes the timestamp, status code, and original URL. Use this to find when a page was first preserved.

Get the first (earliest) capture of a URL
- **get_latest_capture**: Includes timestamp, status code, and URL. Use this to find the newest preserved version of a page.

Get the most recent capture of a URL
- **get_subdomain_captures**: g., *.example.com). Use this to discover the archival footprint of an entire domain, finding all subdomains that have been preserved.

Get captures for all subdomains of a domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Internet Archive Wayback** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if https://example.com has been archived."

**🤖 AI Agent:**
> ✅ URL is archived! Closest snapshot: 20240115120000 (January 15, 2024). View at: https://web.archive.org/web/20240115120000/https://example.com. Total captures: 1,247 over 28 years.

---

**👤 You:**
> "Show me all captures of https://example.com from 2020."

**🤖 AI Agent:**
> Found 52 captures of https://example.com in 2020. First: 2020-01-03 (status 200), Last: 2020-12-28 (status 200). Average capture frequency: ~1 per week. All returned HTTP 200 (OK).

---

**👤 You:**
> "Find all subdomains of archive.org that have been captured."

**🤖 AI Agent:**
> Found captures for 15 subdomains of archive.org: www, web, developer, donate, help, blog, advancedsearch, petabox, us.archive.org, and others. Most captures are from www and web subdomains. Oldest capture dates back to 1998.


## ❓ FAQ

**Q: How far back does the Wayback Machine go?**
The Wayback Machine has archived web pages since 1996. However, coverage varies significantly — major websites have captures going back 20+ years, while smaller or newer sites may have fewer or no captures. Use get_first_capture to find the earliest archived version of any URL.

**Q: Can I find captures that returned 404 errors?**
Yes! Use get_captures_by_status with status_code="404". This returns all archived versions where the page returned a Not Found error. This is useful for tracking when pages were removed or URLs changed structure.

**Q: Can I discover all subdomains of a website that have been archived?**
Yes! Use get_subdomain_captures with the base domain (e.g., "example.com"). This returns captures for all subdomains like www.example.com, blog.example.com, api.example.com, etc. It's useful for mapping the full archival footprint of an organization's web presence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive-wayback](https://vinkius.com/mcp/internet-archive-wayback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Internet Archive Wayback** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `internet-archive-wayback` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Internet Archive Wayback** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "internet-archive-wayback": {
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
