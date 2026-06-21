# Revenue Quality Scorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/revenue-quality-scorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/revenue-quality-scorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/revenue-quality-scorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze revenue stability, concentration risk, and market diversification.

## Description
The Revenue Quality Scorer provides a deep analytical dive into the health of your revenue streams. By evaluating six critical dimensions--including recurring revenue ratio, customer concentration (HHI index), expansion vs new logo mix, contractual stability, geographic diversification, and product diversity--it delivers actionable scores from 0-100. Use `summarize_revenue_quality` for a high-level overview, `analyze_concentration_risk` to identify dependency on large clients, `analyze_contractual_stability` to assess contract longevity, and `analyze_market_breadth` to measure global and product spread.


## Available Tools
- **summarize_revenue_quality**: Summarize revenue quality for a given fiscal year
- **analyze_market_breadth**: Analyze market breadth and diversification
- **analyze_concentration_risk**: Analyze revenue concentration risk
- **analyze_contractual_stability**: Analyze contractual revenue stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Revenue Quality Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of our revenue quality for the 2023 fiscal year."

**🤖 AI Agent:**
> For the 2023 fiscal year, your overall revenue quality score is 78 (PREMIUM). The breakdown includes a high recurring revenue ratio and strong geographic diversification, though there is moderate concentration risk in the North American region.

---

**👤 You:**
> "How much risk are we facing from our largest customers?"

**🤖 AI Agent:**
> The concentration risk analysis shows a score of 65. Your top customer represents 12% of total revenue, which is currently within the manageable range, but monitoring is advised.

---

**👤 You:**
> "Analyze our market breadth in Europe."

**🤖 AI Agent:**
> In the Europe region, your geographic score is 85 and product score is 70. Primary revenue drivers include Enterprise Software and Cloud Services.


## Installation & Usage

To install and use the **Revenue Quality Scorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revenue-quality-scorer](https://vinkius.com/mcp/revenue-quality-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
