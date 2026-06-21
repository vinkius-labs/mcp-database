# Tax Regime Comparator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tax-regime-comparator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tax-regime-comparator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tax-regime-comparator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate and compare Brazilian tax regimes to find the most cost-effective structure for your business.

## Description
The Tax Regime Comparator is a specialized financial simulation engine designed to help businesses navigate the complexities of Brazilian taxation. By analyzing projected annual revenue, profit margins, and business activity types, this MCP server provides precise comparisons between Simples Nacional, Lucro Presumido, and Lucro Real. Use `compare_tax_regimes` to identify the optimal regime and potential savings, or use `get_regime_breakdown` for a granular view of specific tax components like IRPJ and CSLL.


## Available Tools
- **compare_tax_regimes**: Compares different Brazilian tax regimes to find the most efficient one
- **get_regime_breakdown**: Provides a detailed breakdown of tax components for a specific regime


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Regime Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare tax regimes for a service company with 500,000 BRL annual revenue and a 30% profit margin."

**🤖 AI Agent:**
> Based on your inputs, the best regime is Simples Nacional, with an estimated total tax of 45,000 BRL and a potential savings of 12,000 BRL compared to Lucro Presumido.

---

**👤 You:**
> "What is the tax breakdown for Lucro Real in a manufacturing business with 2,000,000 BRL revenue?"

**🤖 AI Agent:**
> For the Lucro Real regime, your total tax is 180,000 BRL. This includes Federal Tax components of 120,000 BRL and Municipal Tax components of 60,000 BRL.

---

**👤 You:**
> "If my profit margin increases to 40%, will the optimal tax regime change?"

**🤖 AI Agent:**
> No, at a 40% profit margin with your current revenue, Simples Nacional remains the most advantageous option.


## Installation & Usage

To install and use the **Tax Regime Comparator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tax-regime-comparator](https://vinkius.com/mcp/tax-regime-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
