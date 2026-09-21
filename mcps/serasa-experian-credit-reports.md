# Serasa Experian Credit Reports MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-reports)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Query the Serasa Experian credit bureau from any AI workflow — PF/PJ credit reports, standalone scores, economic groups and credit rating.

## Description
Connect your **Serasa Experian** account so any AI agent can consult the Brazilian credit bureau directly — using Serasa's official API.

### What you can do

- **PF credit reports** — Básico, Intermediário and Avançado reports for a CPF: registration data, negative annotations (pefin/refin), Serasa queries and score
- **PJ credit reports** — the same family for a CNPJ, plus shareholding and administrative board data
- **Standalone scores** — "Dados Avulsos" PF/PJ: scores and attributes on their own, including SCORE_POSITIVO, SCORE_DE_CREDITO_SETORIAL and SCORE_FRAUDE_PJ
- **Economic groups** — Agrupe: map the economic group a person or company belongs to, with shareholders and subsidiaries
- **Credit rating** — rating and the análise cadastral / análise de balanço family for legal entities

### How it works

`list_credit_reports` returns the exact `report_name` for every family — no credentials needed. Every other tool takes a CPF (11 digits) or CNPJ (14 digits) plus that report name. The server authenticates with your Client ID / Client Secret, caches the 1-hour Bearer token, and switches between production, homologation and sandbox by base URL.


## Available Tools (8)
- **get_pf_economic_group**: Returns the group the person belongs to and its participants. report_name defaults to AGRUPE_PF; use list_credit_reports to see variants (financeiro, participation).

Identify the economic group and its composition starting from a natural person (PF)
- **get_pj_credit_rating**: report_name defaults to RELATORIO_CREDIT_RATING; the family also includes análise cadastral, análise de balanço (normal e consolidado) e versão para instituições financeiras — see list_credit_reports.

Fetch the credit rating / analysis report for a legal entity (PJ)
- **get_pj_economic_group**: Returns whether the company belongs to an economic group and its composition (shareholders, subsidiaries, financial participation). report_name defaults to AGRUPE; variants in list_credit_reports (financeiro, participacoes, QSA, subsidiarias).

Identify the economic group and its composition starting from a legal entity (PJ)
- **get_pj_scores**: Available models include SCORE_DE_CREDITO_SETORIAL (HRS9 — risk of the economic sector), SCORE_POSITIVO (HSUJ), SCORE_FRAUDE_PJ, SCORE_LONGEVIDADE_EMPRESA and SCORE_ATACADISTA. Pass the model via report_parameters, e.g. { "SCORE_POSITIVO": "HSUJ" }.

Fetch standalone scores and attributes for a legal entity (PJ) without a full credit report
- **list_credit_reports**: Call this before any other tool to discover the exact `report_name` string, then pass it to get_pf_report / get_pj_report / get_pf_scores / get_pj_scores / get_pf_economic_group / get_pj_economic_group / get_pj_credit_rating.

List the report names (reportName) available for PF and PJ credit reports, scores, economic groups and credit rating
- **get_pf_report**: `report_name` comes from list_credit_reports (e.g. RELATORIO_BASICO_PF, RELATORIO_INTERMEDIARIO_PF, RELATORIO_AVANCADO_PF). `cpf` must be 11 digits, digits only. `optional_features` adds extra modules when contracted. Some features need `report_parameters` (name→value pairs) — the engine base64-encodes them automatically.

Fetch a full credit report for a natural person (PF) by CPF
- **get_pf_scores**: Use RELATORIO_DADOS_AVULSOS_PF as the report_name. Models include HLRD-family scores; pass the specific model in `report_parameters` (name=SCORE_POSITIVO, value=HSUJ) when the feature requires it.

Fetch standalone scores and attributes for a natural person (PF) without a full credit report
- **get_pj_report**: `report_name` comes from list_credit_reports (e.g. RELATORIO_BASICO_PJ, RELATORIO_INTERMEDIARIO_PJ, RELATORIO_AVANCADO_PJ). `cnpj` must be 14 digits, digits only.

Fetch a full credit report for a legal entity (PJ) by CNPJ


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Experian Credit Reports** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pull the full credit report for CNPJ 33.014.556/0001-96 and summarize its negative annotations and score."

**🤖 AI Agent:**
> I fetched RELATORIO_AVANCADO_PJ. The company has 2 active negative annotations (1 pefin, 1 refin), no protests, and the credit score is 720 of 1000 — risk class C. The shareholding data shows one partner with 90% participation.

---

**👤 You:**
> "What standalone scores are available for this CPF, without a full report?"

**🤖 AI Agent:**
> I ran the Dados Avulsos PF query. The contracted models returned: Serasa Score (SCORE_POSITIVO, HSUJ) 640, and the registration-status attribute showing "Regular". No negative-data features are included in this product — use get_pf_report for those.

---

**👤 You:**
> "Map the economic group behind this CNPJ."

**🤖 AI Agent:**
> I queried Agrupe. This CNPJ belongs to an economic group of 4 companies: the holding company, two subsidiaries, and one related party via shareholding. The group also has a financial-participation link to a fifth company.


## ❓ FAQ

**Q: Where do I get my Serasa Client ID and Client Secret?**
Register and sign in at **developer.serasaexperian.com.br**, then contract the credit-report products you need. Serasa issues a Client ID / Client Secret pair per contract — paste both into the credential fields. Note that the pair only unlocks the report families you actually contracted; a report name you didn't buy returns an authorization error.

**Q: What is the difference between the report families?**
Básico (Crednet family) gives registration data, negative annotations and score. Intermediário (Concentre) adds credit data. Avançado (Credit Bureau for PF, Relato for PJ) is the most complete. "Dados Avulsos" returns only scores and attributes. Agrupe maps economic groups, and Credit Rating returns the rating for legal entities. Call `list_credit_reports` to see the exact `report_name` for each.

**Q: Why did my report call return an authorization error?**
Three common causes: the report family isn't contracted for your Client ID; the base URL doesn't match the environment where your credentials were issued (production vs homologation vs sandbox); or the token expired. The server caches the token for under an hour and re-authenticates automatically, and it clears the cache on a 401 so the next call re-logins. Volumes above your contracted average also trigger a consumption-variation lock — notify Serasa support before bulk runs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-reports](https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-reports)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Experian Credit Reports** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-experian-credit-reports` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Experian Credit Reports** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-experian-credit-reports": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
