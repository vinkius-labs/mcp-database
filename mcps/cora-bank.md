# Cora Bank MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cora-bank)
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


## Available Tools (8)
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


## ❓ FAQ

**Q: How do I encode my Cora `.pem` certificates properly?**
Head to Cora Bank's portal and setup an API App yielding you exactly the Client Credentials and a certificate pairing (Public CERT `.pem`/`.crt` and Private `.key`). Go to a UNIX shell / MacOS Terminal: `base64 -i my_key.key` to get the key text, and `base64 -i my_cert.pem` to get the cert text. The unformatted, unbroken blocks are the credentials you paste directly to us.

**Q: Does Cora produce a separate Pix link from its Boleto command?**
In Cora's domain, executing `cora_create_invoice` natively packages everything. A single entity 'Invoice' acts as both your printable boleto format AND a highly specific Dynamic QR Pix, ensuring multiple avenues for your clients.

**Q: Will an outgoing Pix from my chat be instant?**
Absolutely. Emitting an explicit request down the `cora_send_pix` route connects instantaneously down Cora's active routing engine (Sistema de Pagamentos Instantâneos - SPI/Bacen) draining specific liquidity.

**Q: Can I cancel unpaid user invoices rapidly from MCP?**
Of course! Call upon the unneeded identifier within your chat interface, prompting the logic `cora_cancel_invoice`, pulling the document from global banking registration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cora-bank](https://vinkius.com/mcp/cora-bank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cora Bank** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cora-bank` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cora Bank** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cora-bank": {
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
