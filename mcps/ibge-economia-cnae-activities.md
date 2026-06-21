# IBGE Economia — CNAE Activities MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-economia-cnae-activities)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-economia-cnae-activities-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-economia-cnae-activities-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Navigate Brazil's entire economic taxonomy: 1,332 CNAE activity codes across 21 sectors, 87 divisions, 285 groups — the definitive resource for business classification, compliance, and market analysis.

## Description
Give your AI agent mastery over the **CNAE** — Brazil's official classification of every economic activity, used for tax registration, business licensing, regulatory compliance, and market research.

### What you can do
- **21 Sections (A-U)** — Top-level economic sectors: Agriculture, Mining, Manufacturing, IT, Finance, Health, etc.
- **87 Divisions** — Drill into specific industries within each sector
- **285 Groups & 672 Classes** — Granular business activity classification
- **1,332 Subclasses** — The most specific activity code used on CNPJ (Brazilian business registration)

### Who is this for?
Accountants, compliance officers, fintech developers, market analysts, business registration platforms, and anyone building AI agents for the Brazilian business ecosystem.


## Available Tools
- **list_secoes_cnae**: List all 21 CNAE economic sections (A-U)
- **list_divisoes_cnae**: g., A for Agriculture, C for Manufacturing).

List CNAE divisions within a section
- **list_classes_cnae**: g., 62 for IT activities).

List CNAE classes within a division
- **get_subclasse_cnae**: Get CNAE subclass details
- **list_subclasses_por_classe**: g., 62015).

List all subclasses within a CNAE class


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Economia — CNAE Activities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What CNAE code should I use for a software development company?"

**🤖 AI Agent:**
> 💻 **Software Development — CNAE Codes**

- **6201-5/01** — Custom software development
- **6201-5/02** — Web development
- **6202-3/00** — IT consulting and support
- **6203-1/00** — Software product development

Section J → Division 62 → Group 620 → Class 6201

Most software houses use 6201-5/01 as primary code.

---

**👤 You:**
> "What economic sectors exist under section C (Manufacturing)?"

**🤖 AI Agent:**
> 🏭 **Section C — Manufacturing (24 Divisions)**

10. Food products | 11. Beverages
13. Textiles | 14. Apparel
20. Chemicals | 21. Pharmaceuticals
25. Metal products | 26. Electronics
29. Vehicles | 30. Other transport

Manufacturing is Brazil's largest section with 24 divisions covering 180+ classes.

---

**👤 You:**
> "What is CNAE subclass 4711-3/01?"

**🤖 AI Agent:**
> 🛒 **CNAE 4711-3/01**

**Comércio varejista de mercadorias em geral, com predominância de produtos alimentícios — hipermercados**

Hierarchy:
- Section G: Commerce
- Division 47: Retail trade
- Group 471: Non-specialized retail
- Class 4711-3: Food retail
- Subclass /01: Hypermarkets


## Installation & Usage

To install and use the **IBGE Economia — CNAE Activities** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-economia-cnae-activities](https://vinkius.com/mcp/ibge-economia-cnae-activities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
