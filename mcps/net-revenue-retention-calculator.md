# Net Revenue Retention Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/net-revenue-retention-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/net-revenue-retention-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/net-revenue-retention-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and analyze NRR and GRR metrics across customer cohorts to evaluate subscription health.

## Description
This MCP server provides specialized tools for analyzing recurring revenue retention. Use `calculate_retention_metrics` to compute Net Revenue Retention (NRR) and Gross Revenue Retention (GRR) based on starting MRR, expansion, contraction, and churn. You can also use `get_segment_benchmarks` to retrieve performance targets for Enterprise or SMB segments, and `evaluate_cohort_health` to determine if your cohort's NRR meets specific health benchmarks like 'World Class' or 'Healthy'. It is an essential tool for SaaS finance and operations teams monitoring subscription stability.


## Available Tools
- **calculate_retention_metrics**: Calculates NRR and GRR for a cohort
- **evaluate_cohort_health**: Evaluates cohort health based on NRR
- **get_segment_benchmarks**: Retrieves performance targets for a segment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Net Revenue Retention Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate retention for a cohort with 100k starting MRR, 10k expansion, 5k contraction, and 2k churn in the Enterprise segment."

**🤖 AI Agent:**
> The calculated Net Revenue Retention (NRR) is 103.0% and the Gross Revenue Retention (GRR) is 93.0%.

---

**👤 You:**
> "What are the performance targets for the SMB segment?"

**🤖 AI Agent:**
> For the SMB segment, the target NRR is 100.0% and the target GRR is 95.0%, categorized as a High-Growth tier.

---

**👤 You:**
> "Is an NRR of 125% in the Enterprise segment considered good?"

**🤖 AI Agent:**
> Yes, an NRR of 125.0% for the Enterprise segment is classified as World Class status.


## Installation & Usage

To install and use the **Net Revenue Retention Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/net-revenue-retention-calculator](https://vinkius.com/mcp/net-revenue-retention-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
