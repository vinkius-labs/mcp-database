# Efí Pay (Gerencianet) MCP Server

Generate dynamic Pix charges, issue traditional bank slips (boletos), and check your account balance via Efí Pay.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/efi-pay-gerencianet)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
The **Efí Pay MCP Server** connects your AI agent directly to one of Brazil's largest payment and digital account platforms (formerly Gerencianet). Command your agent to handle invoicing seamlessly using natural language.

### What you can do

- **Pix Management** — Generate dynamic immediate charges (Pix Cob), check specific payment statuses in real-time, and send Pix directly to external keys.
- **Traditional Invoicing** — Emit traditional Brazilian bank slips (Boletos) with specified expiration dates, item totals, and payer documents (CPF/CNPJ).
- **Account Overviews** — Ask your agent to retrieve your current Efí account balance or pull a complete historical banking statement over a defined date range.

### How it works

1. Subscribe to this server.
2. In your Efí Back Office, generate your `Client_ID`, `Client_Secret` and `.p12` Certificate.
3. Convert your `.p12` certificate into a Base64 string.
4. Input the credentials in your MCP-compatible client.

### Who is this for?

- **SaaS Founders** — quickly issue a boleto for a customer directly from your terminal or chat without opening the bank Dashboard.
- **E-commerce Ops** — instantly verify whether a specific Pix `txid` has been paid to fulfill an order right from your internal agent.
- **Financial Controllers** — extract statements and daily balances dynamically to aid reconciliation.


## Available Tools
- **efi_create_boleto**: Gerar um banco slip tradicional brasileiro (Boleto)
- **efi_create_pix_charge**: Emitir cobrança imediata via Pix (Cob)
- **efi_get_balance**: Consultar o resuldado / Saldo atual da conta digital (Efí Pay)
- **efi_get_pix_payment**: Consultar um único pagamento Pix recebido específico
- **efi_get_statement**: Consultar o Resumo (Statement / Extrato) das movimentações da conta
- **efi_list_boletos**: Listar todos os Boletos e transações emitidos em um range de datas
- **efi_list_pix_charges**: Consultar cobranças Pix (Cob) recebidas ou geradas num intervalo
- **efi_send_pix**: Enviar um Pix em tempo real para terceiros


## Installation & Usage

To install and use the **Efí Pay (Gerencianet)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/efi-pay-gerencianet](https://vinkius.com/mcp/efi-pay-gerencianet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
