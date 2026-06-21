# Siteimprove MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/siteimprove)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Monitor and improve your website quality — track accessibility, SEO, content QA, and broken links across your domains with AI agents.

## Description
Connect your **Siteimprove** account to any AI agent to automatically pull website quality scores, accessibility issues, and SEO metrics into your workspace. Turn raw analytics into actionable insights without leaving your chat.

### What you can do

- **Digital Certainty Index (DCI)** — Get a high-level summary of a site's overall quality, accessibility, and SEO health
- **Accessibility (A11y)** — List specific technical accessibility barriers that are causing compliance drops
- **Site Quality Assurance (QA)** — Identify broken links, misspellings, and readability metrics across all crawled pages
- **SEO Oversight** — Retrieve technical SEO errors that are impacting your search engine rankings
- **Fleet Management** — List all monitored sites and browse individual crawled pages

### How it works

1. Subscribe to this server
2. Provide your Siteimprove login Email and API Key
3. Talk to Claude, Cursor, or any MCP-compatible client to request ad-hoc site audits

Stop digging through separate Siteimprove dashboards to figure out why your DCI dropped. Your AI copilot will pinpoint the broken links and accessibility violations instantly.

### Who is this for?

- **Web Accessibility Managers** — quickly request lists of A11y violations for developers to remediate in GitHub
- **SEO Specialists** — track ranking-blocking issues and QA drops across multiple regional domains in a single prompt
- **Front-end Developers** — ask your assistant to pull broken links and accessibility errors while you're coding to fix them proactively


## Available Tools
- **list_sites**: Lists all monitored websites in Siteimprove
- **get_site_details**: Retrieves details for a specific site
- **get_site_summary**: Retrieves the Digital Certainty Index (DCI) overview for a site
- **list_crawled_pages**: Lists all crawled pages for a specific site
- **get_accessibility_summary**: Retrieves the accessibility health overview for a site
- **list_accessibility_issues**: Lists specific accessibility issues discovered on a site
- **get_seo_summary**: Retrieves the SEO health overview for a site
- **get_qa_summary**: Retrieves the Quality Assurance (QA) health overview for a site
- **list_broken_links**: Lists all broken links found on a specific site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Siteimprove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitored sites in my Siteimprove account."

**🤖 AI Agent:**
> I found 3 monitored sites in your Siteimprove account:
1. Acme Corporation Data (ID: 1547844111) - https://acme.org
2. ACME France Store (ID: 1545698711) - https://fr.acme.org
3. Support Desk Portal (ID: 1698782331) - https://support.acme.org

For which site would you like to retrieve the DCI Summary or check broken links?

---

**👤 You:**
> "Get the latest accessibility issues for site 1547844111."

**🤖 AI Agent:**
> There are 4 high-priority accessibility issues on `https://acme.org`:
- Missing `alt` tags on 18 image elements (/blog/new-post)
- Color contrast ratio fails WCAG 2.1 AA on the primary `#header`
- Empty heading elements detected on (/contact)
- Multiple duplicate IDs found across login forms.

Should I group these by page?

---

**👤 You:**
> "What is the DCI Summary score for my main domain?"

**🤖 AI Agent:**
> The overall DCI (Digital Certainty Index) score for your main site is **83.4**.
- QA Score: **91.0**
- SEO Score: **86.2**
- Accessibility Score: **73.0**

The most significant opportunity is improving your Accessibility compliance score. Should I pull the exact issues causing the low accessibility rating?


## ❓ FAQ

**Q: Can my AI automatically detect accessibility barriers on newly crawled pages?**
Yes. Ask the agent to list the accessibility issues for a specific Site ID. It pulls from Siteimprove's latest crawls to pinpoint exact violations (e.g., missing alt text, ARIA label failures), so you can remediate them before the next audit cycle.

**Q: How do I easily fix broken links without searching them all manually?**
Ask your agent to 'list all broken links' on the site. Instead of manually parsing reports, your AI will list the exact origin page where the broken link exists, plus the broken destination URL. You can use this checklist to rapidly go through your CMS and fix them.

**Q: Can my agent give me a quick health summary of my domain?**
Absolutely. Request the 'Digital Certainty Index (DCI) summary' for your site. The agent instantly pulls your overall Quality Assurance score, SEO health, and Accessibility compliance rating, which is perfect for generating a quick weekly status report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/siteimprove](https://vinkius.com/mcp/siteimprove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Siteimprove** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `siteimprove` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Siteimprove** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "siteimprove": {
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
