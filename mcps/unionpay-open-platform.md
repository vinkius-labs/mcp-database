# UnionPay Open Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unionpay-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unionpay-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unionpay-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Bring UnionPay QR Codes and secure global payments to your AI workflow. Handle card verification and online checkout.

## Description
Integrate the world's largest card network directly into your operations. **UnionPay Open Platform** allows your AI agents to programmatically verify identities, tokenize bank cards, and generate interoperable QR payment codes.

### What you can do

- **QR Code Payments** — Generate C2B (Customer-to-Business) unified QR codes for rapid transactions and check their scanning status
- **Tokenization** — Securely handle card binding operations, turning sensitive card details into a safe Token ID for recurring billing
- **KYC & Risk Checks** — Validate combinations of Card Number, ID, and Phone Number directly against the bank's system

### How it works

1. Subscribe to this server
2. Insert your **App ID** and **App Secret** from the [UnionPay Developer Portal](https://developer.unionpayintl.com)
3. Start verifying cardholders and generating checkouts right from your LLM prompt

### Who is this for?

- **Fintech Agents** — Perform primary KYC verifications to quickly qualify user identities
- **Store Managers** — Generate and send dynamic invoices as QR Codes to users instantly in chats
- **Cross-border Developers** — Easily manage Chinese payments globally without complex SDK footprint


## Available Tools
- **cancel_card_token**: Unbind or cancel an existing UnionPay card token
- **check_card_risk_status**: Query UnionPay risk status for a card
- **generate_qr_code**: Generate a UnionPay QR Code for payment
- **get_qr_transaction_status**: Check the payment status of a QR code transaction
- **init_secure_payment**: Initialize a Secure Pay (Online Payment) checkout session
- **request_card_token**: Tokenize a UnionPay card for secure future payments
- **verify_card_kyc**: Verify identity and card binding (KYC)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UnionPay Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a payment QR code for an order of 500 CNY."

**🤖 AI Agent:**
> I've successfully requested the C2B QR Code. Here is the QR Code payload and URL which you can display to your customer.

---

**👤 You:**
> "Check if this UnionPay card is flagged as high-risk: 6222021XXXXXXX."

**🤖 AI Agent:**
> I checked the UnionPay risk registry. This card has not been flagged for fraud and is operating normally.

---

**👤 You:**
> "Cancel the recurring billing Token ID TK-82739."

**🤖 AI Agent:**
> The card binding associated with Token 'TK-82739' has been safely unlinked. Future charges against this token will fail.


## Installation & Usage

To install and use the **UnionPay Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unionpay-open-platform](https://vinkius.com/mcp/unionpay-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
