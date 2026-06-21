# Stark Bank MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stark-bank)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stark-bank-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stark-bank-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI with Brazil's enterprise Developer Bank. Automate corporate virtual cards, Boletos, Outbound Pix (Transfers), and statements inside chats.

## Description
The **Stark Bank MCP Server** brings highest-end Brazilian financial tech directly into your Agent's context. Engineered specifically for complex corporate maneuvers and heavy automations requiring zero filesystem intervention—authentication is fully handled via ECDSA public/private cryptography inside the MCP.

### What you can do

- **Mass Corporate Payables (Transfers)** — You can ask your chatbot to send Pix out to specific people, or execute TED transfers programmatically parsing bank codes and taxes.
- **Asset Generation** — Rapidly generate virtual Corporate Cards or Boletos targeting specific customer strings.
- **Unmatched Oversight** — Check precisely the atomic balance of your Stark accounts or extract statements and invoice status tracking in milliseconds.

### How it works

1. Use your Stark Bank Dashboard to get your `Project ID`.
2. Through your Stark Bank app dashboard or API settings, generate an `ECDSA Private/Public Key`. 
3. Paste the actual raw physical `Private Key` multiline PEM block into your MCP credentials inside your Vinkius application.

### Who is this for?

- **CFOs & Digital Financiers** — Trigger high-volume payment transfers across arrays of workers instantly from the console.
- **Infrastructure Ops** — Rotate corporate cards when limits trigger by simply pinging your AI sidekick.


## Available Tools
- **stark_create_boleto**: Efetuar a emissão de Lote de Boletos Bancários Oficiais (Stark Bank)
- **stark_create_corporate_card**: Tecnologia Enterprise: Criar novo Cartão de Crédito Corporativo on-the-fly
- **stark_create_pix_charge**: Criar uma Cobrança Pix dinâmica imediata (Stark Bank)
- **stark_create_transfer**: INICIAR PAGAMENTOS: Emissão de TED ou Pix para fornecedores/funcionários
- **stark_get_balance**: Consultar resgate atual monetário / total em caixa no banco (Balance)
- **stark_get_statement**: Gerar statement cru detalhado de fluxo de caixa
- **stark_list_boletos**: Listar progressão contábil e status dos Boletos
- **stark_list_pix_charges**: Listar histórico das Cobranças Pix originadas
- **stark_list_transfers**: Descobrir rastreio de pagamentos de saída finalizados (Transfers)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stark Bank** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a dynamic Corporate Card on Stark Bank named 'Google Cloud Pay' for my team."

**🤖 AI Agent:**
> Processing instruction inside Stark ecosystem. Success! A Corporate Card 'Google Cloud Pay' was successfully created on-chain and registered to your active corporate boundary logic.

---

**👤 You:**
> "Extract the detailed historical stark statements spanning from March 1st to March 15th to examine payroll expenditures."

**🤖 AI Agent:**
> I've pulled the 15-day range JSON history. Total observed movements: 21 lines. The main outbound expenditures matched transfers made using out_bound Pix.

---

**👤 You:**
> "Create a Boleto for 500 BRL to CPF 000101111909. It must expire 10 days from today."

**🤖 AI Agent:**
> Boleto initialized inside Stark Bank batch array successfully under the desired CPF target. Check the array payload internally or export the barcode now.


## Installation & Usage

To install and use the **Stark Bank** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stark-bank](https://vinkius.com/mcp/stark-bank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
