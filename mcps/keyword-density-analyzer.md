# Keyword Density Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keyword-density-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Calculate keyword frequency, density percentage, and spatial distribution in text to optimize SEO content.

## Description
The Keyword Density Analyzer connects AI agents to specialized content optimization logic. Use `calculate_keyword_frequency` to find the exact count and density of a target term, `map_keyword_distribution` to identify keyword clustering or uneven spread throughout your document, and `check_density_compliance` to ensure your text stays within the optimal 1% to 3% range for search engine visibility.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keyword Density Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the density of 'SEO' in 'SEO is important for SEO.'?"

**🤖 AI Agent:**
> The keyword 'SEO' appears 2 times, resulting in a density of 66.67%.

---

**👤 You:**
> "Check if a 4% density is optimal."

**🤖 AI Agent:**
> A density of 4.0% is classified as 'High' risk, meaning it exceeds the optimal threshold.

---

**👤 You:**
> "Where does 'target' appear in 'target start target end'?"

**🤖 AI Agent:**
> The keyword 'target' was found at word indices 0 and 2, representing 0.0% and 50.0% through the text.


## ❓ FAQ

**Q: How do I check if my keyword density is too high?**
Use the `check_density_compliance` tool with your calculated percentage to see if it falls into the 'High' risk tier. Tools available: `your_tool_name`.

**Q: Can I see where keywords are located in my text?**
Yes, the `map_keyword_distribution` tool provides the exact word indices and relative positions of every occurrence.

**Q: What is the ideal keyword density?**
For optimal SEO performance, aim for a density between 1% and 3%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keyword-density-analyzer](https://vinkius.com/mcp/keyword-density-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keyword Density Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keyword-density-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keyword Density Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keyword-density-analyzer": {
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
