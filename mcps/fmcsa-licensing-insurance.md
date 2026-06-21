# FMCSA Licensing & Insurance MCP Server

Access real-time FMCSA data to verify motor carrier licensing, insurance, safety ratings, and authority status directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fmcsa-licensing-insurance)

## Overview
**Category:** government-public-data
**Tools Count:** 9

## Description
Connect your AI agent to the **Federal Motor Carrier Safety Administration (FMCSA)** database to perform deep due diligence on trucking companies and motor carriers. This server enables instant retrieval of official government records for compliance, safety, and operational verification.

### What you can do

- **Carrier Identification** — Search for carriers by Legal/DBA name or retrieve specific profiles using U.S. DOT or Docket numbers.
- **Safety & Compliance** — Access Carrier BASIC (Safety) measures and Out-of-Service (OOS) data to evaluate risk.
- **Operating Authority** — Verify the current status of a carrier's operating authority and associated docket numbers.
- **Operational Details** — Inspect authorized cargo types and operation classifications to ensure the carrier matches your logistics needs.

### How it works

1. Subscribe to this server
2. Enter your FMCSA Web Key
3. Start auditing carriers directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — Instantly verify if a new carrier is authorized and insured before booking a load.
- **Compliance Officers** — Automate the monitoring of safety ratings and out-of-service orders for your fleet partners.
- **Freight Brokers** — Streamline the vetting process by pulling government data directly into your workflow.


## Available Tools
- **get_carrier_authority**: Retrieve operating authority status
- **get_carrier_basics**: S. DOT number.

Retrieve Carrier BASIC (Safety) measures
- **get_carrier_by_docket**: Retrieve carrier details by Docket Number
- **get_carrier_by_dot**: S. DOT number.

Retrieve carrier details by U.S. DOT number
- **get_carrier_cargo**: Retrieve types of cargo carried
- **get_carrier_dockets**: Retrieve associated docket numbers
- **get_carrier_oos**: Retrieve Out-of-Service (OOS) data
- **get_carrier_operation_class**: Retrieve operation classifications
- **search_carriers_by_name**: Supports pagination.

Search carriers by Legal or DBA name


## Installation & Usage

To install and use the **FMCSA Licensing & Insurance** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fmcsa-licensing-insurance](https://vinkius.com/mcp/fmcsa-licensing-insurance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
