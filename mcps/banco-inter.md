# Banco Inter MCP Server

Connect to your Banco Inter Empresas digital account. Automate Pix, Boletos, balance inquiries and statements.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/banco-inter)

## Overview
**Category:** money-moves
**Tools Count:** 8

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


## Available Tools
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


## Installation & Usage

To install and use the **Banco Inter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/banco-inter](https://vinkius.com/mcp/banco-inter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
