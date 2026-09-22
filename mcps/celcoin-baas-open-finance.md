# Celcoin BaaS & Open Finance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/celcoin-baas-open-finance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

The Celcoin Open Finance BaaS v2 as an MCP: BaaS accounts, wallet balances, movement statements, registered Pix keys, outgoing Pix and interbank TED transfers with status tracking — OAuth client_credentials bearer, sandbox by default.

## Description
The **Celcoin Open Finance BaaS v2 API** as a single MCP server — a payments console for BaaS partners on Celcoin's Brazilian open finance infrastructure (Pix, TED and wallet operations).

### What you can do
- **Accounts** — list BaaS accounts created in a date window, paginated (account number, document number, balance snapshot)
- **Wallets** — current balance (available, blocked, total) and paginated movement history over a date range
- **Pix** — the Pix keys registered on an account, outgoing Pix (initiation type, immediate/dated, urgency, remittance, end-to-end id) and their live status
- **TED** — interbank same-day transfers with a BACEN finality code and their live status

### Authentication
OAuth2 **client_credentials**: the MCP mints a bearer token at the Celcoin token endpoint (about 40-minute lifetime, auto-refreshed inside the server) and re-mints it once if a call is rejected. Your credentials are only ever used to obtain that token.

### Environments
The sandbox base URL is the default and needs no extra setup — the Celcoin docs publish a public sandbox test pair for the bill payment, recharge or transfer products. The production base URL additionally requires, per Celcoin's docs, an mTLS certificate issued by Celcoin plus a source-IP allowlist; a hosted runner cannot provide either, so production is intended for self-hosted or edge callers that hold the certificate.

### Who is this for
Financial institutions and BaaS operators that run on Celcoin — bill payment, recharges, Pix and TED operations, and agent-driven balance and reconciliation checks.


## Available Tools (9)
- **check_credentials**: Returns the base URL in use, the token type, the token lifetime in seconds (about 40 minutes) and the decoded token claims (subject, issuer, scope) — the subject identifies the integration partner on the account. No account data is involved. Run this first when setting up the MCP or when other tools start failing with authentication errors.

Verify Celcoin credentials by minting a fresh bearer token and report the result
- **pix_payment_status**: Identify the transaction with at least one of: id (the transaction id returned by pix_payment), client_code (the Celcoin client code) or end_to_end_id (the correlation id supplied at initiation). Use it to follow up a payment the user initiated earlier, e.g. "did the Pix go through?"

Check the status of an outgoing Pix initiated with pix_payment
- **list_accounts**: g. "2026-09-01"). Use account or document_number to narrow to one specific account — document_number is the holder's CPF/CNPJ. Page is 1-based; limit_per_page runs 1 to 200. Each record includes the account number, document number, account type and a balance snapshot. Use it to answer "which accounts did we open last month?" and to locate account numbers for the balance, statement and Pix-key tools. Ask for one page at a time and follow up with the next page when the user wants more.

List BaaS accounts created in a date window, paginated
- **get_balance**: account and document_number are optional — pass one or both to target a specific account. Answer "how much is in account X?" or "what is available to move?" with this. The blocked amount is held by pending movements and is not available for transfers.

Get the current balance of a BaaS wallet
- **get_statement**: Each movement includes its description, amount, date and status. account and document_number optionally target one wallet. order is "asc" (oldest first, default) or "desc" (newest first). Walk the history one page at a time with page and limit_per_page instead of requesting everything. Use it for "what went in and out of this account last week?"

Get the paginated movement history of a BaaS wallet over a date range
- **list_pix_keys**: Use it to find an account's receiving key or to check which keys a customer has registered. Pass the account number (find it with list_accounts).

List the Pix keys registered on a BaaS account
- **pix_payment**: amount is a number in BRL (e.g. "25.50"), client_code is the Celcoin client code, and debit_party and credit_party are JSON objects describing the sending and receiving parties. debit_party: {"account","taxId","name","branch","accountType","bank"}. credit_party: {"bank","account","branch","taxId","name","accountType","key"} — either a full account with branch and bank, or a Pix key. initiation_type: "MANUAL" (typing account data), "QR_CODE", "STATIC" or "EMVCO". payment_type: "IMMEDIATE" or "DATED". urgency is optional: "LOW", "MEDIUM" or "HIGH". remittance_information is the free-text memo shown to the receiver. end_to_end_id is an optional correlation id. Returns a transaction id — track it with pix_payment_status. This moves real money: confirm the amount, client code and both parties with the user before calling.

Initiate an outgoing Pix from a BaaS account
- **ted_transfer**: amount is a number in BRL; client_code is the Celcoin client code; client_finality is a BACEN finality code for the transfer purpose (6 digits, e.g. "010101"; "99999" means "other"). debit_party and credit_party are JSON objects in the same shape as the Pix party objects: {"account","taxId","name","branch","accountType","bank"} plus "bank" on the credit side. When client_finality is "99999", description becomes required — it is the free-text purpose shown on the receiver's statement. Returns a transaction id — track it with ted_transfer_status. This moves real money: confirm the amount, client code, finality and both parties with the user before calling.

Initiate a TED (interbank same-day transfer) between bank accounts
- **ted_transfer_status**: Identify it by id (the transaction id returned by ted_transfer) and/or client_code. Use it to follow up an interbank transfer the user initiated earlier.

Check the status of a TED initiated with ted_transfer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Celcoin BaaS & Open Finance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the available balance on account 3214?"

**🤖 AI Agent:**
> 🏦 **Celcoin: Wallet balance**

Available R$ 1,240.50 — blocked R$ 0.00 — total R$ 1,240.50.

Want the movements of this wallet last week, or the Pix keys registered on it?

---

**👤 You:**
> "What went in and out of account 3214 last week?"

**🤖 AI Agent:**
> 📄 **Celcoin: Statement 2026-09-14 to 2026-09-20 (page 1)**

- 09-15 — Pix received R$ 350.00 (JOAO@email.com) — settled
- 09-16 — TED sent R$ 100.00 (finality 010101) — settled
- 09-18 — Bill payment R$ 45.90 (Light S.A.) — settled

Want the next page or a specific day?

---

**👤 You:**
> "Send a Pix of R$ 25.50 from account 3214 to the Pix key joao@email.com, memo "lunch"."

**🤖 AI Agent:**
> Before moving R$ 25.50, confirming the details: from BaaS account 3214, to Pix key joao@email.com, immediate, memo "lunch". Shall I initiate it? After that I can track it with the status tool.


## ❓ FAQ

**Q: Where do I get the Celcoin Client ID and Secret?**
The Celcoin integration team issues them during your homologation. For testing, the Celcoin docs publish a public sandbox test pair for the bill payment, recharge or transfer products — point the base URL at the sandbox and use that pair right away.

**Q: Sandbox or production — which base URL do I set?**
Leave the base URL empty (or set the sandbox URL) to call the sandbox, which needs no extra setup. Per Celcoin's docs, the production base URL additionally requires an mTLS certificate issued by Celcoin plus a source-IP allowlist — a hosted runner cannot provide either, so production is intended for self-hosted or edge callers that hold the certificate.

**Q: Do pix_payment and ted_transfer actually move money?**
Yes — both initiate real BRL transfers in the connected environment (in the sandbox, against sandbox balances). The tools tell the agent to confirm the amount, parties and purpose with you before calling. Track each one afterwards with pix_payment_status or ted_transfer_status.

**Q: What is client_finality in a TED?**
It is the BACEN finality code describing the purpose of the interbank transfer — a 6-digit code such as 010101. "99999" means no specific finality (other), in which case the free-text description becomes required and is what the receiver sees on their statement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/celcoin-baas-open-finance](https://vinkius.com/en/ai-agent-connect/celcoin-baas-open-finance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Celcoin BaaS & Open Finance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `celcoin-baas-open-finance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Celcoin BaaS & Open Finance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "celcoin-baas-open-finance": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
