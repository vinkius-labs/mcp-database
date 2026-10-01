# Portfolio Image Selection Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/portfolio-image-selection-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media-management](../categories/media-management.md)

Ranks portfolio assets using weighted criteria like quality, relevance, and variety.

## Description
This MCP server provides a specialized ranking engine for portfolio management. It allows AI agents to evaluate sets of assets against user-defined weights for five key dimensions: Quality, Relevance, Variety, Recency, and Rights Clearance. Using the `rank_portfolio_assets` tool, agents can identify the optimal selection of images for specific project needs. The system also includes `validate_weight_distribution` to ensure mathematical accuracy and `filter_by_rights_status` to ensure legal compliance for selected assets.


## Available Tools (4)
- **calculate_variety_penalty**: 
- **filter_by_rights_status**: 
- **rank_portfolio_assets**: 0

Ranks portfolio assets based on weighted criteria
- **validate_weight_distribution**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Image Selection Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these assets: [{'id': 'img1', 'quality': 0.9, 'relevance': 0.8, 'variety': 0.5, 'recency': 0.7, 'rights_clearance': 1.0}, {'id': 'img2', 'quality': 0.7, 'relevance': 0.9, 'variety': 0.6, 'recency': 0.4, 'rights_clearance': 1.0}] with weights {'quality': 0.4, 'relevance': 0.4, 'variety': 0.1, 'recency': 0.1, 'rights_clearance': 0.0}"

**🤖 AI Agent:**
> [{'id': 'img1', 'total_score': 0.81}, {'id': 'img2', 'total_score': 0.76}]

---

**👤 You:**
> "Check if these weights are valid: {'quality': 0.5, 'relevance': 0.5}"

**🤖 AI Agent:**
> {"valid": false, "errors": ["variety, recency, and rights_clearance are missing"]}

---

**👤 You:**
> "Filter these assets for full rights: [{'id': 'a1', 'rights_clearance': 1.0}, {'id': 'a2', 'rights_clearance': 0.5}]"

**🤖 AI Agent:**
> [{'id': 'a1', 'rights_clearance': 1.0}]


## ❓ FAQ

**Q: How are the assets ranked?**
Assets are ranked by calculating a total score: the sum of each dimension's score multiplied by its assigned weight. In the event of a tie, the asset with the higher individual quality score is ranked higher.

**Q: Can I ensure my weights are valid?**
Yes, you can use the `validate_weight_distribution` tool to verify that your weights are non-negative and sum exactly to 1.0.

**Q: How does the system handle legal usage?**
The `filter_by_rights_status` tool allows you to filter assets based on a hierarchy of clearance levels: full, limited, or none.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/portfolio-image-selection-score](https://vinkius.com/en/ai-agent-connect/portfolio-image-selection-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Image Selection Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-image-selection-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Image Selection Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-image-selection-score": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
