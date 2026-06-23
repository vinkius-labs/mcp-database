# Core Web Vitals Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/core-web-vitals-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Evaluate LCP, INP, and CLS metrics against Google's thresholds.

## Description
An analytical tool that evaluates web performance metrics (LCP, INP, CLS) against standardized thresholds to provide status classifications, a composite health score, and estimated SEO ranking impact. Use `classify_metric_value` for single metrics, `analyze_performance_suite` for a full overview, and `get_threshold_reference` to see the scoring boundaries.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Core Web Vitals Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the status of an LCP of 2.0 seconds?"

**🤖 AI Agent:**
> An LCP of 2.0 seconds is classified as Good.

---

**👤 You:**
> "Analyze this performance suite: LCP 3s, INP 400ms, CLS 0.3."

**🤖 AI Agent:**
> The analysis shows an overall health score of 50.0 with a Medium ranking impact.

---

**👤 You:**
> "Show me the thresholds for CLS."

**🤖 AI Agent:**
> For CLS, a value up to 0.1 is Good, and up to 0.25 is Needs Improvement.


## ❓ FAQ

**Q: What are Core Web Vitals?**
Core Web Vitals are a set of specific metrics used by Google to measure the user experience of a webpage, focusing on loading speed, responsiveness, and visual stability. Tools available: `your_tool_name`.

**Q: How is the composite score calculated?**
The composite score is a weighted average of your LCP, INP, and CLS statuses. Each metric is assigned a grade: Good (100), Needs Improvement (50), or Poor (0).

**Q: Does this tool affect my SEO?**
While the tool itself doesn't change your site, it provides an estimate of how your current performance metrics might impact your search engine visibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/core-web-vitals-scorer](https://vinkius.com/mcp/core-web-vitals-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Core Web Vitals Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `core-web-vitals-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Core Web Vitals Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "core-web-vitals-scorer": {
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
