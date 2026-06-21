# Cora Bank MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cora-bank)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cora-bank-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cora-bank-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Connect your Cora Corporate account. Have your Ai Assistant generate structured Invoices, Boletos, and Pix codes while tracking active balances.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cora Bank** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Draw up a Cora Invoice for client Gabriel (CPF 908129841). Bill them exactly R$ 150 BRL for the 'Graphic Design Package' with due date at the end of next month."

**🤖 AI Agent:**
> Success. Cora Bank has recognized and generated a formal Invoice. Tracking ID matched. You can supply them with the associated barcode string outputted logically above right now.

---

**👤 You:**
> "Fetch the final Cora Account statement focusing from 2024-04-01 until 2024-04-06 to ensure we captured all vendor payouts."

**🤖 AI Agent:**
> Evaluating API responses constraint: Statement arrays captured exactly 14 operational days log events within that interval. Specifically indicating three substantial outward vendor Pix paths totaling X ammount.

---

**👤 You:**
> "Cancel the Cora pending invoice reference 'INV_17009401' completely. We negotiated an upfront cash structure."

**🤖 AI Agent:**
> Signal passed downwards to cancelation logic. The identified Cora invoice array has been purged and set to 'DELETED_OR_CANCELED'. Barcodes will bounce if the user attempts scanning them.


## Installation & Usage

To install and use the **Cora Bank** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cora-bank](https://vinkius.com/mcp/cora-bank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
