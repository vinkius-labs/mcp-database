# Geekflare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geekflare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test your website performance, security headers, and DNS configuration with a comprehensive suite of technical audit tools.

## Description
Connect your **Geekflare** account to any AI agent and simplify how you monitor website performance, secure your domains, and analyze SEO health through natural conversation.

### What you can do

- **Audit & SEO** — Run full Google Lighthouse audits to measure speed, accessibility, and search engine optimization.
- **Performance Testing** — Measure server response times (TTFB) and overall page load speed to identify bottlenecks.
- **Security Scanning** — Analyze SSL/TLS certificates for validity and security vulnerabilities in real-time.
- **Network Intelligence** — Retrieve DNS records (A, MX, CNAME, TXT) and Whois registration data for any domain.
- **Link Oversight** — Automatically identify broken links (404s) on any page to improve user experience.
- **Visual Monitoring** — Capture full-page screenshots of target URLs programmatically via AI.
- **Operational Visibility** — Verify API health and monitor your digital infrastructure directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Geekflare API Key (found in your account dashboard)
3. Start auditing your web presence from Claude, Cursor, or any MCP client

### Who is this for?

- **Web Developers & DevOps** — quickly check SSL status and measure page speed via simple AI commands.
- **SEO Specialists** — run Lighthouse audits and identify broken links directly from the workspace.
- **IT Managers** — verify DNS records and monitor domain ownership details via the AI assistant.


## Available Tools
- **check_broken_links**: Identify broken links on a page
- **get_dns_records**: Retrieve DNS records
- **run_lighthouse_audit**: Run Lighthouse SEO/Performance audit
- **measure_load_time**: Measure page speed and TTFB
- **take_website_screenshot**: Capture a website screenshot
- **scan_ssl_tls_cert**: Scan SSL/TLS certificate
- **get_whois_data**: Retrieve Whois information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geekflare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a Lighthouse audit for 'https://google.com'."

**🤖 AI Agent:**
> Audit complete! Google.com has the following scores: Performance (95), SEO (100), Accessibility (92), and Best Practices (100). Would you like the detailed breakdown of performance issues?

---

**👤 You:**
> "Check for broken links on 'https://example.com/blog'."

**🤖 AI Agent:**
> Scanning for broken links... I found 2 broken links on the page: 'https://example.com/old-post' (404) and 'https://example.com/deleted-image.png' (404). Shall I check other pages on this site?

---

**👤 You:**
> "What are the MX and A records for 'apple.com'?"

**🤖 AI Agent:**
> Fetching DNS data... For apple.com, I found A records pointing to 17.253.144.10 and MX records for apple-com.mail.protection.outlook.com. Would you like to see the TXT or CNAME records as well?


## ❓ FAQ

**Q: Can I run a full Lighthouse SEO audit via AI?**
Yes! Use the `run_lighthouse_audit` tool and provide the target URL. Your agent will return scores for Performance, SEO, Accessibility, and Best Practices.

**Q: How do I check if my SSL certificate is valid using the agent?**
Use the `scan_ssl_tls_cert` tool. Provide the domain name, and Geekflare will verify the issuer, expiration date, and security protocols used by your site.

**Q: Is it possible to see the DNS records for a domain via AI?**
Absolutely. Use the `get_dns_records` query. Provide the URL, and the agent will retrieve A, MX, CNAME, and TXT records registered for that domain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geekflare](https://vinkius.com/mcp/geekflare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geekflare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `geekflare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geekflare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geekflare": {
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
