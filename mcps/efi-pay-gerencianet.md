# Efí Pay (Gerencianet) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/efi-pay-gerencianet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Generate dynamic Pix charges, issue traditional bank slips (boletos), and check your account balance via Efí Pay.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Efí Pay (Gerencianet)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a dynamic Pix charge of R$ 150.00 expiring in 3600 seconds, and link it to my external key myemail@store.com."

**🤖 AI Agent:**
> The Pix charge has been generated successfully. Your transaction ID (txid) is '8b8f[...]'. The copy-paste literal string and dynamic BR Code is available below for your customer.

---

**👤 You:**
> "Check the status of the Pix payment holding the txid 'abc123zxy456'."

**🤖 AI Agent:**
> Fetching payment status... The Pix transaction 'abc123zxy456' is marked as 'CONCLUIDA' (Confirmed). The funds have landed in your total balance.

---

**👤 You:**
> "Pull a list of my generated Boletos since September 1st, showing me only the unpaid ones."

**🤖 AI Agent:**
> I've pulled the data! You generated 24 Boletos since September 1st, but exactly 6 remain active and unpaid across various clients.


## ❓ FAQ

**Q: How do I setup my Base64 Certificate and API credentials?**
Log into your Efí account, go to **API > Applications**. Create an app to get the Client ID and Secret. Then generate a Production Certificate (`.p12`). Instead of uploading the file to Vinkius, use terminal command `base64 -i your_cert.p12` to convert it into a plaintext string, and paste that robust text directly into the MCP configuration.

**Q: Can I automatically verify if a customer paid a Pix charge just by chatting with my AI?**
Yes! Provide the agent the exact transaction id (`txid`) of the generated Pix. The agent will query the `efi_get_pix_payment` tool and immediately tell you if the status is active, answered, or expired.

**Q: Does the integration support transferring money out (Cash-out)?**
Yes. Using the `efi_send_pix` action, you can initiate outbound immediate payments requesting the agent to process a value directly to a receiver Pix key.

**Q: Can I query a history of paid bank slips (Boletos) at the end of the day or month?**
Certainly. The `efi_list_boletos` and `efi_get_statement` tool allows you to perform large queries parsing begin/end dates to return summaries directly in your terminal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/efi-pay-gerencianet](https://vinkius.com/mcp/efi-pay-gerencianet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Efí Pay (Gerencianet)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `efi-pay-gerencianet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Efí Pay (Gerencianet)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "efi-pay-gerencianet": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
