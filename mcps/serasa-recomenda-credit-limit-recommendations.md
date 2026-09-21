# Serasa Recomenda — Credit Limit Recommendations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-recomenda-credit-limit-recommendations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate credit-grant decisions and recommended limits for CPF and CNPJ across nine distribution channels.

## Description
Recomenda is Serasa Experian's decision-as-a-service for credit granting. Submit a CPF or CNPJ with the operation amount and receive a proposal number, a recommended credit limit, a risk level and a sales orientation. This connector covers all nine distribution channels — direct, distribuidor, distribuidor_prorede, ecommerce, ecommerce_relatorio, erp, erp_relatorio, consumo_externo and large — each with its own request path and accepted fields. Unsupported optional fields for the chosen channel are dropped automatically so a request never fails on a schema mismatch. Optional enrichment modules (score, negative annotations, estimated revenue or income) are selected through informacoes_adicionais. Proposals can be retrieved individually, listed with history on e-commerce channels, and exported as a recommendations report. Authentication is OAuth2 client credentials issued at developer.serasaexperian.com.br.


## Available Tools (4)
- **generate_recommendations_report**: With no filters it returns the whole base, so narrow it with nome/cnpj/data_inicio/data_fim/user_id/status/numero_proposta. Status codes are 04, 06 and 07.

Export a report of PJ (CNPJ) recommendations, filterable by name, document, proposal number, user or status
- **get_proposal**: " identifier returned by recommend_credit_limit. Pass the same channel and document_type used at creation so the request hits the right path.

Fetch a previously generated recommendation by its proposal number (numeroProposta)
- **list_proposals**: Filters: `busca` matches name or document, `status` matches the recommendation status, and `data_inicio` / `data_fim` bound the creation date (ISO 8601). Page with pagina_atual / tamanho_pagina (defaults 0 and 5). Use this to recover a proposal number before get_proposal.

List the credit recommendations already generated, with date, document and status filters
- **recommend_credit_limit**: `channel` is the distribution model of the proposal — pick the one that matches how the credit is sold: direct, distribuidor, distribuidor_prorede, ecommerce, ecommerce_relatorio, erp, erp_relatorio, consumo_externo or large.

`cod_tipo_venda`: 1 = new customer, 2 = recurring customer. `politica`: 1 or 2 (risk policy version). Not every channel accepts every optional field — unsupported ones for the chosen channel are dropped automatically. `informacoes_adicionais` selects extra modules as a JSON object, e.g. {"anotacoesCompletas": true, "rendaEstimada": true, "faturamentoEstimado": true}.

Generate a credit-grant recommendation and suggested credit limit for a CPF or CNPJ


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Recomenda — Credit Limit Recommendations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend a credit limit for CNPJ 33014556000196 for a 1500 operation on the direct channel, recurring customer."

**🤖 AI Agent:**
> Calls recommend_credit_limit with channel direct, document_type PJ, document 33014556000196, valor_operacao 1500 and cod_tipo_venda 2, then returns the proposal number, recommended limit, risk level and sales orientation.

---

**👤 You:**
> "What limit would Serasa suggest for this new customer, including score and negative annotations?"

**🤖 AI Agent:**
> Calls recommend_credit_limit with cod_tipo_venda 1 and informacoes_adicionais {"anotacoesCompletas": true} so score and negative-annotation modules come back with the recommendation.

---

**👤 You:**
> "List the proposals we generated for that CNPJ through the distributor-prorede channel."

**🤖 AI Agent:**
> Calls list_proposals with channel distribuidor_prorede and document_type PJ, which hits the flat /distribuidor-prorede/propostas path and returns the stored proposals.


## ❓ FAQ

**Q: Which channel should I use?**
The channel mirrors how the credit is sold: direct for your own sales team, distribuidor or distribuidor_prorede for a dealer network, ecommerce / ecommerce_relatorio for online checkout, erp / erp_relatorio when the request comes from an ERP, consumo_externo for third-party consumption and large for high-value operations.

**Q: Why was my optional field ignored?**
Each channel's schema accepts only a subset of the optional fields. The connector drops whatever the chosen channel does not support — for example parceiro is only valid on consumo_externo and large, and documento_indireto only on distribuidor_prorede — so the request stays valid.

**Q: What does cod_tipo_venda mean?**
It marks the sale type: 1 for a new customer and 2 for a recurring customer. Combined with politica (1 or 2, the risk policy version) it selects which decision policy Serasa applies to the proposal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-recomenda-credit-limit-recommendations](https://vinkius.com/en/ai-agent-connect/serasa-recomenda-credit-limit-recommendations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Recomenda — Credit Limit Recommendations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-recomenda-credit-limit-recommendations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Recomenda — Credit Limit Recommendations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-recomenda-credit-limit-recommendations": {
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
