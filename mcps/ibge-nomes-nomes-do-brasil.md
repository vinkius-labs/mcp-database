# IBGE Nomes — Nomes do Brasil MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-nomes-nomes-do-brasil)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-nomes-nomes-do-brasil-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-nomes-nomes-do-brasil-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Discover the history behind every Brazilian name: birth frequency by decade since the 1930s, national popularity rankings, and regional trends — the viral dataset that captivated 200 million Brazilians.

## Description
Tap into Brazil's most **viral dataset** — the IBGE Names API that broke the internet when launched, as 200 million Brazilians rushed to look up their own names.

### What you can do
- **Name Frequency** — How many "Marias" were born in each decade since 1930? Track any name's rise and fall across almost 100 years
- **National Ranking** — Top 20 most popular names by decade + filter by sex (M/F)
- **Regional Trends** — Compare name popularity across Brazilian states (is "José" more popular in Bahia or São Paulo?)

### Who is this for?
Baby name apps, genealogy platforms, marketing professionals, data journalists, cultural researchers, and anyone building engaging Brazilian content.


## Available Tools
- **get_nome_frequencia**: Supports multiple names separated by |. Example: "Maria", "João|Pedro".

Get birth frequency by decade for a Brazilian name
- **get_ranking_nomes**: Can be filtered by decade and/or sex (M or F).

Get ranking of most popular names in Brazil
- **get_nome_por_localidade**: Use the IBGE UF code (e.g., 33 for RJ, 35 for SP).

Get name frequency filtered by Brazilian state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Nomes — Nomes do Brasil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How popular was the name 'Maria' across decades in Brazil?"

**🤖 AI Agent:**
> 👩 **Maria — Frequency by Decade**

1930s: 336,477 births
1950s: 1,487,301 births (peak! 🔝)
1970s: 1,225,640 births
1990s: 562,893 births
2010s: 145,301 births

Maria was Brazil's #1 name for 60 years but has declined 90% since its 1950s peak.

---

**👤 You:**
> "What are the top 10 baby names in Brazil in the 2000s?"

**🤖 AI Agent:**
> 🏆 **Top 10 Names — 2000s Decade**

1. Maria (562K) | 2. Ana (345K)
3. João (289K) | 4. Pedro (267K)
5. Lucas (254K) | 6. Gabriel (248K)
7. Mateus (210K) | 8. Guilherme (195K)
9. Rafael (188K) | 10. Mariana (172K)

Biblical names dominate, with Lucas and Gabriel surging.

---

**👤 You:**
> "Is 'João' more popular in Bahia or in Rio Grande do Sul?"

**🤖 AI Agent:**
> 📊 **João — Regional Comparison**

🏖️ Bahia: 892K total births (since 1930)
🍷 Rio Grande do Sul: 456K total births

João is **nearly 2× more popular** in Bahia than in Rio Grande do Sul, reflecting the Northeast's stronger tradition of Biblical naming.


## Installation & Usage

To install and use the **IBGE Nomes — Nomes do Brasil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-nomes-nomes-do-brasil](https://vinkius.com/mcp/ibge-nomes-nomes-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
