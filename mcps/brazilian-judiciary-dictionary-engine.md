# Brazilian Judiciary Dictionary Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Detect every Brazilian court, tribunal, agency, and regulatory body mentioned in legal documents — 100+ pre-indexed entities with zero AI inference.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brazilian Judiciary Dictionary Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan this 300-page litigation bundle and tell me exactly which Brazilian courts and agencies are referenced."

**🤖 AI Agent:**
> Scan complete. Found 9 entities: STJ (45 mentions), TJSP (23), TRF3 (18), CADE (12), MPF (8), CNJ (5), TRT2 (4), ANVISA (3), AGU (2). Category summary: {"Superior": 45, "TJ": 23, "TRF": 18, "Regulador": 15, "MP/Advocacia": 10, "Controle": 5, "TRT": 4}.

---

**👤 You:**
> "I need to know how many times each TRT appears in this labor law case file to determine jurisdictional concentration."

**🤖 AI Agent:**
> Analysis complete. TRT2 (São Paulo — Capital) leads with 34 mentions, TRT15 (Campinas) has 12, TRT1 (Rio de Janeiro) has 8, and TST has 19. Category breakdown: {"TRT": 54, "Superior": 19}.

---

**👤 You:**
> "Check if any regulatory agency (CADE, CVM, BACEN, ANVISA) is mentioned in this corporate compliance report."

**🤖 AI Agent:**
> Found 4 regulatory entities: BACEN (22 mentions), CVM (15), CADE (9), SUSEP (3). No mention of ANVISA. Category summary: {"Regulador": 49}.


## ❓ FAQ

**Q: What exactly is pre-indexed?**
The complete Brazilian judiciary: 5 Superior Courts, 6 TRFs, 24 TRTs, 27 TJs (including TJDFT), 3 military TJMs, oversight bodies (CNJ, CNMP, TCU), prosecution and advocacy (AGU, MPF, MPT, MPM, MPDFT, DPU, OAB), and 15 regulatory agencies (CADE, CVM, BACEN, INPI, INSS, SUSEP, ANATEL, ANVISA, ANS, ANAC, ANEEL, ANP, ANA, ANTT, ANTAQ).

**Q: Does it cover courts from other countries?**
No. This engine covers exclusively the Brazilian legal system. To add courts from other countries, pass a custom JSON dictionary mapping acronyms to full names. Custom entries are tagged separately in the output.

**Q: How are results organized?**
Each detected entity includes its acronym, full official name, category (Superior, TRF, TRT, TJ, TJM, Controle, MP/Advocacia, Regulador), and exact mention count. A category summary is also provided for quick analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine](https://vinkius.com/mcp/brazilian-judiciary-dictionary-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brazilian Judiciary Dictionary Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `brazilian-judiciary-dictionary-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brazilian Judiciary Dictionary Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brazilian-judiciary-dictionary-engine": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
