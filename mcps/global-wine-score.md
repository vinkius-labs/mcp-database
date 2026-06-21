# Global Wine Score MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/global-wine-score)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/global-wine-score-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/global-wine-score-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access aggregated wine ratings from the world's top critics — normalized scores, vintage analysis, and top-rated wine discovery through natural conversation.

## Description
Connect to **Global Wine Score** and access the most objective wine rating system — scores aggregated and normalized from the world's leading critics.

### What you can do

- **Wine Scores** — Search any wine and get its aggregated score (0-100) with confidence index
- **Latest Ratings** — Browse the most recently published scores from top critics worldwide
- **By Color** — Filter by Red, White, Rosé, or Sparkling to find the best in each category
- **By Country** — Explore top-rated wines from France, Italy, USA, Spain, Australia, and more
- **By Vintage** — Compare vintages to identify exceptional years and investment opportunities
- **Top Wines** — Discover elite wines scoring 95+ from a consensus of respected critics

### How it works

Global Wine Score aggregates ratings from **Parker (Wine Advocate), Wine Spectator, Jancis Robinson, Vinous, Decanter**, and other major publications. Each wine receives a single normalized score with a confidence index based on the number and consistency of reviews.

### Who is this for?

- **Sommeliers** — Quick score checks during wine list curation and guest recommendations
- **Wine Collectors** — Investment-grade wine discovery and vintage comparison
- **Wine Importers** — Identify rising stars and verify quality across regions
- **Enthusiasts** — Data-driven wine exploration beyond single-critic bias


## Available Tools
- **get_latest_scores**: ). Each score is a confidence-weighted average out of 100, with vintage and regional context.

Get latest wine scores
- **search_wine_scores**: Returns all matching wines with their normalized score (0-100), confidence index, vintage, color, country, and regions. The primary tool for answering "what score did X get?"

Search scores for a wine
- **scores_by_color**: Returns top-rated wines of that style, sorted by score. Perfect for "what are the best white wines right now?"

Get scores by wine color
- **scores_by_country**: Returns top-rated wines from that country. For regional exploration and comparison.

Get scores by country
- **scores_by_vintage**: Returns top-rated wines from a specific harvest. Essential for vintage comparison and investment decisions.

Get scores by vintage
- **get_top_scores**: The absolute elite — wines rated exceptional by a consensus of the world's most respected critics. For collectors and investment-grade wine discovery.

Get top-rated wines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Global Wine Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the highest-rated Italian wines of 2020?"

**🤖 AI Agent:**
> ⭐ **Top Italian Wines — 2020 Vintage**

1. **Masseto 2020** — Toscana
   ⭐ **98/100** 🎯 Confidence: Very High
   🍷 Red | 📍 Bolgheri

2. **Sassicaia 2020** — Tenuta San Guido
   ⭐ **97/100** 🎯 Confidence: Very High
   🍷 Red | 📍 Bolgheri

3. **Barolo Monfortino 2016** — Giacomo Conterno
   ⭐ **97/100** 🎯 Confidence: High
   🍷 Red | 📍 Barolo

4. **Tignanello 2020** — Antinori
   ⭐ **96/100** 🎯 Confidence: Very High
   🍷 Red | 📍 Toscana

---

**👤 You:**
> "Compare the scores for Château Margaux 2015 and 2016."

**🤖 AI Agent:**
> Château Margaux 2015 has an outstanding aggregated score of 98.7/100, while the 2016 vintage received an almost perfect consensus of 99.1/100, both with a Very High confidence index.

---

**👤 You:**
> "Find the top-rated California Cabernet Sauvignon from 2018."

**🤖 AI Agent:**
> The top-rated California Cabernet Sauvignon from 2018 is Promontory by Harlan Estate, boasting an aggregated Global Wine Score of 98.5/100 with a High confidence rating.


## Installation & Usage

To install and use the **Global Wine Score** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/global-wine-score](https://vinkius.com/mcp/global-wine-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
