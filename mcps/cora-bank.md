# Cora Bank MCP Server

Connect your Cora Corporate account. Have your Ai Assistant generate structured Invoices, Boletos, and Pix codes while tracking active balances.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cora-bank)

## Overview
**Category:** finance-accounting
**Tools Count:** 8

## Description
The **Cora Bank MCP Server** attaches your corporate entity directly to your AI programming or conversational agent via officially supported backend APIs. 

### What you can do

- **Invoicing Power** — Utilize native `cora_create_invoice` to print a highly detailed digital invoice that simultaneously displays a standard Brazilian Boleto barcode and a Pix QR code for max conversion mapping.
- **Payment Outs** — Fire `cora_send_pix` securely via text interactions without opening separate mobile applications to clear out daily vendor tabs.
- **Status Overviews** — Keep track of unread metrics through statements queries, canceling generated invoices smoothly.

### How it works

1. Use your administrative panel to declare an API generation target within Cora.
2. The mTLS standard issues your unique Private `.key` and Application `.pem/.crt` files to your native computer. 
3. Because uploading key files directly isn't optimal on Vinkius, use your Terminal string encoder (`base64 -i my_certificate.pem`) to collapse the keys into two blocks of string payloads.
4. Save these inside your Vinkius application to bridge access safely.

### Who is this for?

- **Independent Studios** — Automatically check if a freelance customer paid their invoice to deliver the product immediately through chat.
- **Retail Ops** — Bulk cancel or modify overdue tickets on conversation flow commands.


## Available Tools
- **cora_cancel_invoice**: Cancela uma cobrança (Invoice) pendente do Banco Cora
- **cora_create_invoice**: Criar uma Cobrança Oficial (Boleto bancário + QR Code Pix) (Cora Bank)
- **cora_get_balance**: Traz todos os recursos atuais parados ou pendentes no Cora Bank.

Consulta de recursos retidos totais (Balanço / Saldo)
- **cora_get_invoice**: Consultar os dados ou status detalhado de uma Fatura/Cobrança
- **cora_get_statement**: Extração de histórico contábil, recebimentos e extrato de cashflow
- **cora_list_invoices**: Lista em massa faturas/boletos e verifica seus resultados
- **cora_list_payments**: Consultar um array contendo os retiros efetuados da sua base ou conta
- **cora_send_pix**: Efetuar envio de TED ou Pix pagando Fornecedor ou Cliente


## Installation & Usage

To install and use the **Cora Bank** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cora-bank](https://vinkius.com/mcp/cora-bank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
