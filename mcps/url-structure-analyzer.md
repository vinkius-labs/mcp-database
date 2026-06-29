# URL Structure Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-structure-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Evaluate web URLs for SEO health, analyzing path depth, keyword relevance, and parameter noise.

## Description
The URL Structure Analyzer is a specialized utility designed to assess the SEO-friendliness of web URLs. By examining key structural elements like directory depth, total character length, and query parameter clutter, it provides an optimization score and actionable alerts. Use `validate_url_input` to ensure your URL is syntactically correct, then apply `analyze_url_structure` with a target keyword to see how well your slug performs. You can also use `retrieve_optimization_benchmarks` to understand the scoring thresholds used for depth, length, and parameter counts.


## Available Tools (3)
- **analyze_url_structure**: Performs the primary structural assessment of the URL and generates an optimization score
- **retrieve_optimization_benchmarks**: Provides the current standard thresholds used for the scoring logic
- **validate_url_input**: ng., http or https) and a valid domain/host.

Ensures the provided string is a syntactically valid URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL Structure Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this URL optimized: https://fashion-hub.com/products/shoes/running-shoes?size=10&color=blue"

**🤖 AI Agent:**
> The URL has a score of 65. Alerts: High directory depth and excessive query parameters detected.

---

**👤 You:**
> "Check if 'running' is in this URL: https://fitness-blog.com/blog/running-tips"

**🤖 AI Agent:**
> The keyword 'running' was found in the slug. Optimization score: 95.

---

**👤 You:**
> "What are the current SEO benchmarks for URL analysis?"

**🤖 AI Agent:**
> The maximum recommended depth is 3, the optimal length is 75 characters, and the parameter threshold is 2.


## ❓ FAQ

**Q: What does the optimization score represent?**
The score (0-100) represents how well a URL follows SEO best practices regarding structure, length, and clarity.

**Q: How can I check for keyword relevance?**
When using `analyze_url_structure`, provide a `targetKeyword` parameter to see if that specific term exists within the URL slug.

**Q: What are 'alerts' in the analysis?**
Alerts are human-readable warnings that highlight specific issues, such as excessive directory depth or too and many query parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-structure-analyzer](https://vinkius.com/mcp/url-structure-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL Structure Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `url-structure-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL Structure Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-structure-analyzer": {
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
