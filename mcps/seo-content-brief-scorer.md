# SEO Content Brief Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seo-content-brief-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Audit content briefs for SEO health, keyword placement, and heading hierarchy.

## Description
The SEO Content Brief Scorer is an automated auditing tool designed to evaluate content briefs against established SEO best practices before the writing process begins. By analyzing structural elements like title length, keyword integration in H1/H2 headings, and semantic heading hierarchy, it identifies optimization gaps that could impact search engine rankings. Use `calculate_brief_score` to get an overall health score and prioritized adjustments, `analyze_keyword_placement` to check keyword coverage in high-impact zones, and `audit_heading_hierarchy` to ensure a logical nesting order of header tags.


## Available Tools (3)
- **analyze_keyword_placement**: Determine how effectively target keywords are integrated into high-impact structural zones
- **audit_heading_hierarchy**: g., H2 to H4) and redundant heading text.

Verify that the content structural outline follows a logical nesting order
- **calculate_brief_score**: Calculate the overall SEO health score for a content brief


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEO Content Brief Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if this content brief is SEO-ready? Title: 'Best Running Shoes 2024', Keywords: ['running shoes', 'marathon training'], Headings: [{'tag': 'H1', 'text': 'Best Running Shoes 2024'}, {'tag': 'H2', 'text': 'Marathon Training Tips'}], Word Count: 1500"

**🤖 AI Agent:**
> The brief is in the Optimal tier with a high SEO health score. Your target keywords are well-placed in the H1 and H2 headings.

---

**👤 You:**
> "Analyze the keyword placement for this brief: Title: 'SEO Guide', Keywords: ['seo strategy', 'backlinks'], Headings: [{'tag': 'H1', 'text': 'SEO Guide'}, {'tag': 'H2', 'text': 'Introduction'}]"

**🤖 AI Agent:**
> The coverage rate is 0%. The keywords 'seo strategy' and 'backlinks' are not found in the title or high-impact H1/H2 headings.

---

**👤 You:**
> "Check this heading structure for errors: [{'tag': 'H1', 'text': 'Main Title'}, {'tag': 'H3', 'text': 'Subtopic'}]"

**🤖 AI Agent:**
> The hierarchy is invalid. The tool detected skipped levels: H2 was bypassed.


## ❓ FAQ

**Q: What does the SEO health score represent?**
The score (0-100) represents how well your brief follows SEO best practices, including title optimization, keyword presence in key headings, and proper heading hierarchy.

**Q: How can I improve my brief's score?**
Use the `calculate_brief_score` tool to receive a list of `priorityAdjustments`. Common fixes include adding missing keywords to H1/H2 tags or fixing broken heading sequences.

**Q: Does this tool check for keyword stuffing?**
The tool focuses on coverage and placement. It identifies if keywords are missing from critical zones like the title or H1/H2 headings using `analyze_keyword_placement`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seo-content-brief-scorer](https://vinkius.com/mcp/seo-content-brief-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEO Content Brief Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seo-content-brief-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEO Content Brief Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seo-content-brief-scorer": {
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
