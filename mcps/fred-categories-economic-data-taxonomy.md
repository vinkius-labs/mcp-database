# FRED Categories — Economic Data Taxonomy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-categories-economic-data-taxonomy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fred-categories-economic-data-taxonomy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fred-categories-economic-data-taxonomy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Navigate the complete FRED taxonomy: from Money & Banking to Employment to Prices — drill down through categories, discover thousands of series organized by topic, and filter by tags and frequency.

## Description
Explore FRED like a library. The Categories server lets your AI agent navigate the entire FRED taxonomy tree — from the root down to individual series.

### What you can do
- **Browse the Tree** — Start from root (category 0) and drill into 8 top-level domains
- **Discover Series** — Find all series within any category, sorted by popularity
- **Tag Filtering** — Get tags for any category to understand available dimensions

### Top-Level Categories
`32991` Money, Banking & Finance · `10` Population & Employment · `32992` National Accounts · `1` Production & Business · `32455` Prices · `32263` International · `33060` Academic Data

### Who is this for?
Data explorers, researchers discovering what data FRED has, and AI agents that need structured navigation of economic indicators.


## Available Tools
- **get_category**: Root category is 0. Major categories: 32991 (Money, Banking, & Finance), 10 (Population, Employment, & Labor Markets), 32992 (National Accounts), 1 (Production & Business Activity), 32455 (Prices).

Get a FRED category by ID
- **get_category_children**: Start from root (0) to explore all top-level categories, then drill down. This is the primary way to discover what data FRED has.

Get child categories of a FRED category
- **get_category_series**: Use with category IDs discovered via get_category_children. Supports filtering by frequency, units, and tags.

Get series within a FRED category
- **get_category_tags**: Useful for understanding what data dimensions are available and for filtering series.

Get tags for a FRED category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FRED Categories — Economic Data Taxonomy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the main categories of economic data in FRED?"

**🤖 AI Agent:**
> 🗂️ **FRED Root Categories**

1. Money, Banking & Finance (32991)
2. Population, Employment & Labor (10)
3. National Accounts (GDP) (32992)
4. Production & Business Activity (1)
5. Prices (32455)
6. International Data (32263)
7. U.S. Regional Data (70)
8. Academic Data (33060)

---

**👤 You:**
> "What inflation-related series are available?"

**🤖 AI Agent:**
> 📈 **Prices Category (32455) — Top Inflation Series**

- CPIAUCSL — Consumer Price Index (All Urban)
- CPILFESL — Core CPI (Ex Food & Energy)
- PCEPI — PCE Price Index
- T10YIE — 10-Year Breakeven Inflation
- MICH — U. Michigan Inflation Expectations

3,000+ price-related series available in this category.

---

**👤 You:**
> "Navigate to the interest rates subcategory"

**🤖 AI Agent:**
> 🏦 **Interest Rates → Children**

- Treasury Constant Maturity (22)
- LIBOR Rates (33003)
- Federal Funds (118)
- Prime Rate (120)
- Swap Rates (33023)

Drill into any to see individual series.


## Installation & Usage

To install and use the **FRED Categories — Economic Data Taxonomy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-categories-economic-data-taxonomy](https://vinkius.com/mcp/fred-categories-economic-data-taxonomy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
