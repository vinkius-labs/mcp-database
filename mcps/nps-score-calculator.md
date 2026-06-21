# NPS Score Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nps-score-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nps-score-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nps-score-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Calculate Net Promoter Score, performance tiers, and statistical margin of error.

## Description
The NPS Score Calculator MCP server provides a complete toolkit for analyzing customer loyalty. Use `calculate_nps` to transform raw response counts into a meaningful Net Promoter Score, including performance classifications (Critical, OK, Good, Excellent) and statistical margin of error. You can also use `get_industry_benchmark` to find standard targets for sectors like Technology or Retail, and `compare_performance` to see how your results stack up against the industry baseline.


## Available Tools
- **get_industry_benchmark**: Retrieves the NPS benchmark for a specific industry
- **calculate_nps**: Calculates Net Promoter Score (NPS) and statistical margin of error
- **compare_performance**: Compares current NPS against industry benchmark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NPS Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my NPS score from these responses: 10 people gave a 10, 5 people gave a 9, 2 people gave an 8, and 3 people gave a 5."

**🤖 AI Agent:**
> Your NPS score is 60. This falls into the 'Good' classification, with a total of 20 responses and a calculated margin of error.

---

**👤 You:**
> "What is the benchmark for the Retail industry?"

**🤖 AI Agent:**
> The standard NPS benchmark for the Retail industry is 30.

---

**👤 You:**
> "Compare an NPS of 45 in the Technology sector to the industry standard."

**🤖 AI Agent:**
> Your NPS of 45 is 15 points above the Technology industry benchmark of 30.


## Installation & Usage

To install and use the **NPS Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nps-score-calculator](https://vinkius.com/mcp/nps-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
