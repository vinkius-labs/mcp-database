# Senado Federal MCP Server

Access real-time data from the Brazilian Federal Senate — track legislative proposals, senator profiles, and mandate histories.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/senado-federal)

## Overview
**Category:** knowledge-management
**Tools Count:** 21

## Description
Connect to the **Senado Federal** Open Data API to monitor the Brazilian legislative process directly through your AI agent. Get transparency and deep insights into the upper house of the National Congress.

### What you can do

- **Senator Profiles** — List current senators, those on leave, and access detailed metadata including party affiliations and historical positions.
- **Legislative Proposals (Matérias)** — Search for specific proposals, track their current status, and view the complete history of movements and actions.
- **Rapporteur Tracking** — Identify which senators are assigned as rapporteurs for specific bills and proposals.
- **Legislative History** — Explore current and historical legislatures to understand the evolution of Brazilian law.
- **Mandate Analysis** — Inspect the full history of mandates and political roles held by any parliamentarian.

### How it works

1. Subscribe to this server
2. Use 'PUBLIC' or your preferred identifier as the access key
3. Start querying the Brazilian Senate database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly verify senator backgrounds and the status of controversial bills.
- **Legal Professionals** — track the progress of legislative changes that affect specific sectors.
- **Civic Tech Developers** — integrate official government data into applications with ease.


## Available Tools
- **get_comissao_composicao**: Get current members of a committee
- **get_comissao**: Get detailed information about a specific committee
- **get_legislatura_atual**: Get details of the current legislature
- **get_legislatura**: Get details of a specific legislature
- **get_materia_movimentacoes**: Get history of actions on a proposal
- **get_materia_relatorias**: Get rapporteurs assigned to a proposal
- **get_materia**: Get detailed information about a specific proposal
- **get_senador_cargos**: Get positions held by a senator
- **get_senador_filiacoes**: Get party affiliations of a senator
- **get_senador_mandatos**: Get mandates held by a senator
- **get_senador**: Get detailed information about a specific senator
- **get_votacao**: Get details of a specific vote
- **list_agenda_reuniao**: List scheduled committee meetings
- **list_agenda_sessao**: List scheduled sessions
- **list_comissoes**: List all committees
- **list_legislaturas**: List all legislatures
- **list_materias_atualizacoes**: List recently updated legislative proposals
- **list_materias_tipos**: g., PL, PEC).

List types of legislative proposals
- **list_senadores_afastados**: List senators currently on leave
- **list_senadores_atual**: List senators currently in office
- **list_votacoes**: List recent votes


## Installation & Usage

To install and use the **Senado Federal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/senado-federal](https://vinkius.com/mcp/senado-federal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
