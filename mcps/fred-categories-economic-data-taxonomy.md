# FRED Categories — Economic Data Taxonomy MCP Server

Navigate the complete FRED taxonomy: from Money & Banking to Employment to Prices — drill down through categories, discover thousands of series organized by topic, and filter by tags and frequency.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-categories-economic-data-taxonomy)

## Overview
**Category:** brain-trust
**Tools Count:** 4

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


## Installation & Usage

To install and use the **FRED Categories — Economic Data Taxonomy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-categories-economic-data-taxonomy](https://vinkius.com/mcp/fred-categories-economic-data-taxonomy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
