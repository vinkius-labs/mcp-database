# Câmara dos Deputados (v2) MCP Server

Access real-time data from the Brazilian Chamber of Deputies — track expenses, speeches, and legislative activities of all deputies.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/camara-dos-deputados-v2)

## Overview
**Category:** knowledge-management
**Tools Count:** 49

## Description
Connect to the **Chamber of Deputies Open Data API** to monitor the Brazilian legislative branch. This server allows AI agents to query detailed information about deputies, their spending, and their political performance through natural conversation.

### What you can do

- **Deputy Profiles** — Search for deputies by name, party, state, or legislature and get full biographical details.
- **Expense Tracking (CEAP)** — Monitor the use of the Parliamentary Quota (CEAP), filtering by year, month, and supplier CNPJ.
- **Legislative Activity** — Access transcripts of speeches, participation in events, and membership in committees or organs.
- **Political Affiliations** — List parliamentary fronts and historical mandate data for any deputy.
- **Professional Background** — Inspect declared professions and previous occupations of elected officials.

### How it works

1. Subscribe to this server
2. No API key is required as it uses public open data
3. Start auditing legislative data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly extract spending data and speech transcripts for investigative reporting.
- **Political Analysts** — monitor party movements, committee memberships, and parliamentary front activities.
- **Civic Tech Developers** — integrate official Brazilian legislative data into transparency tools and dashboards.


## Available Tools
- **get_bloco**: Get details of a block
- **get_deputado**: Get details of a specific deputy
- **get_evento**: Get details of an event
- **get_frente**: Get details of a parliamentary front
- **get_orgao**: Get details of an organ
- **get_partido**: Get details of a party
- **get_proposicao**: Get details of a proposition
- **get_votacao**: Get details of a specific voting
- **list_blocos**: List active parliamentary blocks
- **list_deputado_despesas**: List expenses reimbursed via Parliamentary Quota for a deputy
- **list_deputado_discursos**: List transcripts of speeches made by the deputy
- **list_deputado_eventos**: List events the deputy participated in
- **list_deputado_frentes**: List parliamentary fronts the deputy belongs to
- **list_deputado_historico**: List historical data of the deputy mandates
- **list_deputado_ocupacoes**: List professional occupations of the deputy
- **list_deputado_orgaos**: List committees and other organs the deputy is a member of
- **list_deputado_profissoes**: List declared professions of the deputy
- **list_deputados**: List deputies (deputados)
- **list_despesas_cota**: Search for expenses across multiple deputies (CEAP)
- **list_evento_deputados**: List deputies present at the event
- **list_evento_orgaos**: List organs responsible for the event
- **list_evento_pauta**: List the agenda (items to be discussed/voted) for an event
- **list_evento_votacoes**: List votings that occurred during the event
- **list_eventos**: List events (sessions, hearings, meetings)
- **list_frente_membros**: List members of the parliamentary front
- **list_frentes**: List parliamentary fronts
- **list_legislatura_mesa**: List members of the Board of Directors for that legislature
- **list_legislaturas**: List legislatures (four-year periods of parliamentary work)
- **list_orgao_membros**: List current members and their roles in the organ
- **list_orgao_votacoes**: List votings held within the organ
- **list_orgaos**: List organs (Committees, Councils, Board of Directors)
- **list_partido_membros**: List deputies currently or previously affiliated with the party
- **list_partidos**: List political parties
- **list_proposicao_autores**: List authors of the proposition
- **list_proposicao_relacionadas**: List other propositions related to this one
- **list_proposicao_temas**: List areas of interest/themes associated with the proposition
- **list_proposicao_tramitacoes**: List history of the proposition progress
- **list_proposicao_votacoes**: List votings related to the proposition
- **list_proposicoes**: List propositions (projects of law, amendments, etc)
- **list_ref_deputados_sigla_uf**: List state abbreviations
- **list_ref_eventos_cod_situacao_evento**: List status codes for events
- **list_ref_eventos_cod_tipo_evento**: List types of events
- **list_ref_orgaos_cod_tipo_orgao**: List types of organs
- **list_ref_proposicoes_cod_situacao**: List status codes for propositions
- **list_ref_proposicoes_cod_tema**: List theme codes for propositions
- **list_ref_proposicoes_sigla_tipo**: List types of propositions (PEC, PL, etc)
- **list_votacao_orientacoes**: List voting recommendations given by party leaders
- **list_votacao_votos**: List individual votes cast by deputies (for nominal votings)
- **list_votacoes**: List votings


## Installation & Usage

To install and use the **Câmara dos Deputados (v2)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/camara-dos-deputados-v2](https://vinkius.com/mcp/camara-dos-deputados-v2)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
