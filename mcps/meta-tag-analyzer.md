# Meta Tag Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meta-tag-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Validate HTML title and meta description tags for SEO optimization.

## Description
The Meta Tag Analyzer MCP server provides a specialized toolkit for SEO professionals to audit HTML metadata. Using tools like `analyze_title` and `analyze_description`, you can verify character counts, estimated pixel widths, and keyword presence to prevent SERP truncation. The `check_redundancy` tool identifies potential keyword stuffing by flagging duplicate terms, while `calculate_seo_score` provides a holistic optimization grade based on all metrics. This server acts as a bridge between your AI agent and professional SEO auditing workflows.


## Available Tools (4)
- **analyze_description**: Evaluates the structural integrity of the meta description tag
- **analyze_title**: Evaluates the structural integrity of the HTML title tag
- **calculate_seo_score**: Generates a final optimization grade
- **check_redundancy**: Identifies repetitive words that may indicate keyword stuffing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meta Tag Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this title: 'Best SEO Tools 2024' with the keyword 'SEO'."

**🤖 AI Agent:**
> The title analysis is complete. Character count: 19. Status: Optimal. The keyword 'SEO' was successfully detected.

---

**👤 You:**
> "Check if my description is too long: 'This is a very long description that might exceed the recommended character limit for search engines and cause truncation in the results page.'"

**🤖 AI Agent:**
> The description analysis shows a status of 'Too Long' due to exceeding the recommended pixel width and character thresholds.

---

**👤 You:**
> "Are there any redundant words in my title 'SEO Tips for SEO Experts' and description 'Learn SEO tips to become an SEO expert'?"

**🤖 AI Agent:**
> The redundancy check identified duplicate terms: ['SEO', 'tips', 'expert']. A high redundancy score was detected.


## ❓ FAQ

**Q: How does the pixel width estimation work?**
The tool estimates horizontal space based on character density and common font metrics to predict if your title or description will be truncated in search results.

**Q: Can I check for specific keywords?**
Yes, when using `analyze_title` or `analyze_description`, you can provide a `primaryKeyword` to verify its presence in your metadata.

**Q: What is included in the SEO score?**
The `calculate_seo_score` tool evaluates keyword presence, length compliance (character and pixel), and the absence of term redundancy to generate a final grade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meta-tag-analyzer](https://vinkius.com/mcp/meta-tag-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meta Tag Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meta-tag-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meta Tag Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meta-tag-analyzer": {
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
