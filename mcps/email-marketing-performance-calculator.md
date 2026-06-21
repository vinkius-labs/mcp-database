# Email Marketing Performance Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/email-marketing-performance-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/email-marketing-performance-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/email-marketing-performance-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and benchmark key email marketing metrics like delivery, engagement, and revenue.

## Description
This MCP server provides specialized tools to quantify the effectiveness of your email campaigns. Use `calculate_delivery_metrics` to determine delivery and open rates, or `calculate_engagement_metrics` to analyze CTOR and conversion efficiency. You can also use `calculate_revenue_metrics` to find revenue per email sent and `get_industry_benchmark` to compare your performance against standard benchmarks for SaaS, eCommerce, Media, and B/B2B industries.


## Available Tools
- **get_industry_benchmark**: Get industry performance benchmarks
- **calculate_delivery_metrics**: Calculate email delivery and open rates
- **calculate_engagement_metrics**: Calculate email engagement metrics
- **calculate_revenue_metrics**: Calculate email revenue metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Marketing Performance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my delivery metrics: 10000 sent, 9500 delivered, 2500 opened."

**🤖 AI Agent:**
> The `calculate_delivery_metrics` tool would return a delivery rate of 95% and an open rate of 26.32%.

---

**👤 You:**
> "What is the benchmark for conversionRate in eCommerce?"

**🤖 AI Agent:**
> The `get_industry_benchmark` tool returns a standard conversion rate of 2.5% for the eCommerce industry.

---

**👤 You:**
> "Calculate engagement: 2500 opened, 400 clicks, 100 conversions, 9500 delivered."

**🤖 AI Agent:**
> The `calculate_engagement_metrics` tool would return a CTOR of 16% and a conversion rate of 1.05%.


## Installation & Usage

To install and use the **Email Marketing Performance Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/email-marketing-performance-calculator](https://vinkius.com/mcp/email-marketing-performance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
