# Rule of 40 Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rule-of-40-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rule-of-40-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rule-of-40-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and benchmark Rule of 40 performance for SaaS and software companies.

## Description
The Rule of 40 Analyzer is a specialized financial tool designed to evaluate the health of software and SaaS businesses. By combining revenue growth rates with profitability margins (EBITDA or FCF), it provides a single metric to assess business efficiency. Use `calculate_rule_of_40` to determine if a company falls into the Risk, Healthy, or Elite performance tiers. For a more comprehensive view, use `compute_ttm_metrics` to aggregate quarterly data and identify long-term trends over the last twelve months. Additionally, you can benchmark your results against industry standards using `compare_to_sector_peers`, which compares your score against established sectors like Software (SaaS), Fintech, and Infrastructure/Cloud.


## Available Tools
- **compare_to_sector_peers**: Compares a company score against industry benchmarks
- **compute_ttm_metrics**: Aggregates quarterly data to determine the TTM performance score
- **calculate_rule_of_40**: g., 40 for 40%) and returns the score and performance tier.

Calculates the Rule of 40 score for a single period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rule of 40 Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Rule of 40 score for a company with 35% revenue growth and 10% EBITDA margin."

**🤖 AI Agent:**
> The Rule of 40 score is 45%, which places the company in the Healthy performance tier.

---

**👤 You:**
> "How does a company with a 70% score compare to the Software (SaaS) sector average?"

**🤖 AI Agent:**
> A score of 70% is significantly above the Software (SaaS) sector average, showing a positive benchmark gap.

---

**👤 You:**
> "Analyze my quarterly performance: [{ growthRate: 40, margin: 5 }, { growthRate: 38, margin: 7 }, { growthRate: 35, margin: 10 }, { growthRate: 30, margin: 12 }]"

**🤖 AI Agent:**
> The TTM Rule of 40 score is 45% with a declining trend status.


## Installation & Usage

To install and use the **Rule of 40 Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rule-of-40-analyzer](https://vinkius.com/mcp/rule-of-40-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
