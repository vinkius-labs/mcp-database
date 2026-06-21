# BCB Inflação — IPCA, IGP-M, INPC e Expectativas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-inflacao-ipca-igp-m-inpc-e-expectativas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bcb-inflacao-ipca-igp-m-inpc-e-expectativas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bcb-inflacao-ipca-igp-m-inpc-e-expectativas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Brazilian inflation indices: IPCA (official CPI), IPCA-15 (advance reading), IGP-M (rent and contract index), INPC (minimum wage index), and Focus Survey market expectations for future inflation from Brazil's Central Bank.

## Description
Brazilian inflation data.

### 5 Tools
- **IPCA** — Official consumer price index
- **IPCA-15** — Advance inflation reading
- **IGP-M** — General price index (rent benchmark)
- **INPC** — Consumer price index (wages)
- **Focus Expectations** — Market forecasts


## Available Tools
- **get_ipca**: Usado como meta de inflação pelo BCB. Mede a variação de preços de uma cesta de consumo para famílias com renda de 1 a 40 salários mínimos. Série SGS: 433.

Obter o IPCA — Índice Nacional de Preços ao Consumidor Amplo
- **get_ipca15**: Muito acompanhado pelo mercado como antecipação do IPCA. Série SGS: 7478.

Obter o IPCA-15 — prévia da inflação oficial
- **get_igpm**: Usado como indexador de aluguéis e contratos. Composição: 60% IPA (atacado) + 30% IPC (consumo) + 10% INCC (construção). Série SGS: 189.

Obter o IGP-M — Índice Geral de Preços - Mercado
- **get_inpc**: Mede a inflação para famílias com renda de 1 a 5 salários mínimos. Usado como referência para reajustes salariais e do salário mínimo. Série SGS: 188.

Obter o INPC — Índice Nacional de Preços ao Consumidor
- **get_expectativas_inflacao**: Filtre por indicador: IPCA, IGP-DI, IGP-M. Inclui mediana, média, mínimo, máximo e desvio padrão.

Obter as expectativas do mercado para a inflação (Relatório Focus)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCB Inflação — IPCA, IGP-M, INPC e Expectativas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current inflation rate in Brazil?"

**🤖 AI Agent:**
> 📊 **IPCA — Brazil Official Inflation**

March 2026: +0.56%
12-month: 5.12%

IPCA is Brazil's official CPI, targeting families with 1-40 minimum wages. The BCB inflation target for 2026 is 3.0% ± 1.5pp.

Source: BCB/IBGE, SGS series 433

---

**👤 You:**
> "What does the Focus market summary expect for the next IPCA?"

**🤖 AI Agent:**
> The median expectation for IPCA year-end stands at 3.90%, according to the latest consultation among Top-5 survey participants.

---

**👤 You:**
> "Track the IGP-M accumulated value this month."

**🤖 AI Agent:**
> The rental inflation tracker, IGP-M, retreated slightly by -0.15% pulling the 12-month accumulated down to an adjusted 4.83%.


## Installation & Usage

To install and use the **BCB Inflação — IPCA, IGP-M, INPC e Expectativas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-inflacao-ipca-igp-m-inpc-e-expectativas](https://vinkius.com/mcp/bcb-inflacao-ipca-igp-m-inpc-e-expectativas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
