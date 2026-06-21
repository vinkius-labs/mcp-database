# ALESP (Assembleia SP) MCP Server

Access open data from the Legislative Assembly of São Paulo, including deputy info, expenses, and legislative proposals.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alesp-assembleia-sp)

## Overview
**Category:** data-analytics
**Tools Count:** 18

## Description
Connect to the **ALESP (Assembleia Legislativa do Estado de São Paulo)** open data portal to monitor legislative activities in real-time. This MCP server allows AI agents to query official information about state deputies, cabinet expenses, committee meetings, and the full lifecycle of legislative proposals.

### What you can do

- **Deputy Tracking** — List all current state deputies and their political affiliations directly from the official registry.
- **Financial Transparency** — Query reimbursed cabinet expenses for any deputy, with support for historical data by year.
- **Legislative Progress** — Track the status, authors, and full history of proposals, bills, and other documents.
- **Committee Monitoring** — Access details about permanent committees, including their members, meetings, and voting records.
- **Administrative Data** — Inspect the organizational structure, staff placements, and job history within the assembly.

### How it works

1. Subscribe to this server
2. No complex API keys are required for this public data source
3. Start auditing legislative transparency from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly gather data on deputy expenses and voting patterns for reporting.
- **Legal Professionals** — monitor the progress of specific bills and legislative norms in real-time.
- **Citizens & Activists** — promote transparency by easily accessing public records through natural conversation.


## Available Tools
- **get_agenda_eventos**: List upcoming and past events scheduled at the Assembly
- **get_comissoes_membros**: List members of the permanent committees
- **get_comissoes_reunioes**: List meetings of the permanent committees
- **get_comissoes**: List permanent committees of the assembly
- **get_comissoes_votacoes**: List votes of the permanent committees
- **get_deputados**: List all state deputies in the current legislature
- **get_despesas_gabinetes**: Optionally provide a year for historical data.

List reimbursed expenses for each deputy cabinet
- **get_documento_andamento_atual**: Get current status of proposals
- **get_documento_andamento**: Get full history and status of proposals
- **get_documento_autor**: List authors and co-signers for each legislative document
- **get_funcionarios_cargos**: List job history of ALESP staff
- **get_legislacao_normas**: List state norms (laws, decrees, resolutions)
- **get_legislacao_temas**: List themes/topics of state norms
- **get_legislacao_tipo_normas**: List types of state norms
- **get_lotacoes**: List current placements (lotações) of ALESP staff
- **get_partidos**: List political parties participating in the legislative process
- **get_proposituras_zip_url**: Get the URL for the comprehensive list of all legislative proposals (ZIP)
- **get_uas**: List Administrative Units (UAs) of ALESP


## Installation & Usage

To install and use the **ALESP (Assembleia SP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alesp-assembleia-sp](https://vinkius.com/mcp/alesp-assembleia-sp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
