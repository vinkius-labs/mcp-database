# SEO On-Page Copy Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seo-on-page-copy-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-tools](../categories/marketing-tools.md)

Analyze keyword density, meta tag truncation, and heading coverage for SEO optimization.

## Description
The SEO On-Page Copy Analyzer provides a suite of tools to audit your web content. Use `analyze_keyword_density` to check for keyword stuffing, `validate_meta_tags` to predict SERP truncation, `audit_heading_coverage` to verify heading hierarchy, and `evaluate_tfidf_significance` to measure keyword importance.


## Available Tools (4)
- **analyze_keyword_density**: Analyze keyword density and prominence in text
- **audit_heading_coverage**: Check for target keywords in page headings
- **validate_meta_tags**: Check if meta title and description are likely to be truncated
- **evaluate_tfidf_significance**: Calculate TF-IDF scores for keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEO On-Page Copy Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the SEO for https://my-blog.com/post: 'SEO is essential for success. SEO helps ranking.'"

**🤖 AI Agent:**
> The density for 'SEO' is 40%. No stuffing detected.

---

**👤 You:**
> "Check if this title will truncate: 'Comprehensive Guide to SEO Optimization in 2024 and Beyond'"

**🤖 AI Agent:**
> The estimated width is 620px. Truncation predicted.

---

**👤 You:**
> "Are keywords present in these headings? [{'tag': 'h1', 'content': 'Best SEO Tools'}]"

**🤖 AI Agent:**
> Keyword 'SEO' was found in the H1 heading.


## ❓ FAQ

**Q: How can I check if my keywords are overused?**
Use the `analyze_keyword_density` tool to identify density percentages and detect potential keyword stuffing.

**Q: Will my meta description be cut off in Google results?**
The `validate_meta_tags` tool estimates pixel width to predict if your title or description will be truncated.

**Q: Can I verify my H1 and H2 tags contain target keywords?**
Yes, the `audit_heading_coverage` tool scans headings for specific keyword presence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seo-on-page-copy-analyzer](https://vinkius.com/mcp/seo-on-page-copy-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEO On-Page Copy Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seo-on-page-copy-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEO On-Page Copy Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seo-on-page-copy-analyzer": {
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
