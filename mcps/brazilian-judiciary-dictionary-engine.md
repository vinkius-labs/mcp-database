# Brazilian Judiciary Dictionary Engine MCP Server

Detect every Brazilian court, tribunal, agency, and regulatory body mentioned in legal documents — 100+ pre-indexed entities with zero AI inference.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine)

## Overview
**Category:** knowledge-management
**Tools Count:** 1

## Description
Language models consistently fail to accurately identify and count legal entity acronyms in large document sets. This engine performs strict, deterministic regex boundary matching against the complete Brazilian judiciary.

### What Is Included

- **5 Tribunais Superiores:** STF, STJ, TST, TSE, STM
- **6 TRFs:** TRF1 through TRF6
- **24 TRTs:** TRT1 (RJ) through TRT24 (MS)
- **27 TJs:** Every State Court including TJDFT
- **3 TJMs:** Tribunais de Justiça Militar (MG, RS, SP)
- **Órgãos de Controle:** CNJ, CNMP, TCU
- **Ministério Público e Advocacia:** AGU, MPF, MPT, MPM, MPDFT, DPU, OAB
- **Agências Reguladoras:** CADE, CVM, BACEN, INPI, INSS, SUSEP, ANATEL, ANVISA, ANS, ANAC, ANEEL, ANP, ANA, ANTT, ANTAQ

### What Is NOT Included

This engine covers exclusively the Brazilian judiciary and regulatory apparatus. Courts from other countries (US, UK, EU, etc.) are not included. Use the custom dictionary parameter to add entities from any other jurisdiction.

### How It Works

- Pure local regex with word boundary matching — zero AI, zero false positives.
- Results grouped by category (Superior, TRF, TRT, TJ, Regulador, etc.).
- Extensible via custom JSON dictionary for additional entities.


## Available Tools
- **search_legal_entities**: Searches text for known legal entities (courts, tribunals) using a strict offline dictionary


## Installation & Usage

To install and use the **Brazilian Judiciary Dictionary Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine](https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
