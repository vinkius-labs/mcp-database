# Banco Inter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/banco-inter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Connect to your Banco Inter Empresas digital account. Automate Pix, Boletos, balance inquiries and statements.

## Description
The **Banco Inter MCP Server** transforms your AI agent into a secure, fully automated financial assistant directly tethered to your Banco Inter Corporate account. Perform high-velocity API commands without ever logging into the Internet Banking portal.

### What you can do

- **Pix Engine** — Interrogate the status of issued billing, generate complex dynamic Pix charges (Pix Cob), and seamlessly orchestrate automated money transfers directly natively through your chatbot.
- **Boleto (Bank Slips)** — Generate fully structured Brazilian bank slips parsing customer identifiers (CPF/CNPJ). You can also extract individual slip histories.
- **Routine Banking** — Access daily statements (Extratos), balance verifications, and general cash flow history queries natively embedded into conversations.

### How it works

1. Use your corporate Banco Inter app to generate your `API Scopes` and Security Certificates (`.crt` and `.key`).
2. The Brazilian BACEN system requires mTLS (Mutual TLS). Instead of downloading server files, you will just Base64 encode both `.crt` and `.key` files.
3. Securely set these long strings as environment credentials in your MCP host.

### Who is this for?

- **Finance Engineers** — Automate tedious manual account checking and boleto generations instantly.
- **Corporate Administrators** — Monitor daily income seamlessly during chat sessions with AI models without security compromises.


## Available Tools (8)
- **inter_create_boleto**: Gerar um Boleto de Cobrança Bancário (Banco Inter)
- **inter_create_pix_billing**: Obrigatório incluir cpfCnpj e valor.

Emitir cobrança imediata via Pix (Banco Inter)
- **inter_get_balance**: Consultar o Saldo final do dia na Conta Digital (Banco Inter Empresas)
- **inter_get_boleto**: Consultar dados detalhados e status de um Boleto específico (Banco Inter)
- **inter_get_statement**: Consultar o Resumo (Statement / Extrato) completo de movimentações da conta (Banco Inter Empresas)
- **inter_list_boletos**: Listar pesquisa filtrada de Boletos em lote (Banco Inter)
- **inter_list_pix_billings**: Consultar cobranças Pix (Cob) recebidas ou geradas num intervalo (Banco Inter)
- **inter_send_pix**: O token deve constar o scope necessário.

Pagamentos - Enviar um Pix utilizando sua Conta Banco Inter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Banco Inter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an Inter corporate Boleto for John Doe (CPF 12345678909). The value is 50.00 expiring on 2026-10-10."

**🤖 AI Agent:**
> The Boleto has been physically recorded in your Banco Inter registry! Nosso Numero corresponds to '[ID]'. The active Barcode string is: '00000.00000.00[...]' which can be forwarded.

---

**👤 You:**
> "Send a dynamic Pix (Cash outbound) of R$ 5.00 to CPF key 03928139."

**🤖 AI Agent:**
> Processing the outgoing transfer... Successfully sent R$ 5.00 to the parsed CPF via Banco Inter rails. Your current liquidity accounts correctly mirror this change.

---

**👤 You:**
> "Load my historical Banco Inter statement (Extrato) from 01/20/2024 to 01/25/2024 and identify if there was any Pix received."

**🤖 AI Agent:**
> Data Extracted. In your historical statements you observed exactly 8 inbound transactions. Three of these lines reflect an inbound automated Pix flow valued at R$ [Total].


## ❓ FAQ

**Q: How do I configure my Banco Inter Base64 Certificates during setup?**
Log into Banco Inter Empresas > **Aplicações** > New application. Select all API scopes (Boleto, Pix, Banking). Download your keys (`.crt` and `.key`). To input them securely without uploading files, run `base64 -i your_cert.crt` and `base64 -i your_cert.key` in your local terminal. Copy-paste these two respective massive text outputs into the `CERT_BASE64` and `KEY_BASE64` MCP connection variables.

**Q: Can I initiate a Pix transfer (send money) out of my corporate account?**
Yes, using the native `inter_send_pix` tool your agent has technical capabilities to make outbound transfers. Proceed with immense caution while deploying agents capable of draining liquidity implicitly.

**Q: Are boletos automatically registered with the 'Nosso Numero' tag upon creation?**
Yes. Banco Inter API automatically parses the request creating a fully valid and verified registered bank slip payload containing the barcode vector dynamically.

**Q: Will checking my bank statement count towards rate limits?**
Banco Inter developer APIs employ basic rate limitations on requests. Using `inter_get_statement` sparingly throughout an automated chat retains total compliance to the quotas without blocking integrations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/banco-inter](https://vinkius.com/mcp/banco-inter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Banco Inter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `banco-inter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Banco Inter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "banco-inter": {
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
