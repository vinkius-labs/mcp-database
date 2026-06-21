# ANVISA (Portal de APIs) MCP Server

Access official Brazilian health regulatory data — query medicines, prices, food registrations, cosmetics, and sanitizers directly from ANVISA.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/anvisa-portal-de-apis)

## Overview
**Category:** government-public-data
**Tools Count:** 7

## Description
Connect to the official **ANVISA (Brazilian Health Regulatory Agency)** API portal and integrate critical health regulatory data into your AI workflows.

### What you can do

- **Medicine Search** — Query registered medicines by commercial name, active ingredient, or registration number using `consultar_medicamentos`.
- **Pricing Intelligence** — Fetch maximum consumer prices (PMC) and factory prices (PF) for regulated drugs via `precos_medicamentos`.
- **Food & Nutrition** — Access the database of registered food products (`registros_alimentos`) and those requiring only notification (`notificacoes_alimentos`).
- **Cosmetics & Hygiene** — Verify registration data for perfumes, hygiene products, and cosmetics using `consultar_cosmeticos`.
- **Sanitizing Products** — Search for cleaning and sanitizing products registered with the agency via `consultar_saneantes`.
- **Pharmacopeia Standards** — Retrieve official monographs for chemical substances and health standards using `monografias_farmacopeia`.

### How it works

1. Subscribe to this server
2. Enter your ANVISA API Key
3. Start querying Brazilian regulatory data from Claude, Cursor, or any MCP client

### Who is this for?

- **Healthcare Professionals** — quickly verify medicine registrations and official pricing without manual portal searches
- **Regulatory & Compliance Teams** — automate the monitoring of food and cosmetic registrations to ensure market compliance
- **Pharmaceutical Researchers** — access Farmacopeia monographs and active ingredient data directly within research environments


## Available Tools
- **consultar_cosmeticos**: Search for registered cosmetic products
- **consultar_medicamentos**: Search for medicines by name, active ingredient, or registration number
- **consultar_saneantes**: Search for registered sanitizing products
- **monografias_farmacopeia**: Retrieve monographs for chemical substances
- **notificacoes_alimentos**: Access food products that only require notification
- **precos_medicamentos**: Retrieve maximum consumer prices (PMC) and factory prices (PF) for medicines
- **registros_alimentos**: List food products registered with ANVISA


## Installation & Usage

To install and use the **ANVISA (Portal de APIs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anvisa-portal-de-apis](https://vinkius.com/mcp/anvisa-portal-de-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
