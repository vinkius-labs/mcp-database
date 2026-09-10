# Claro Insight (Marketplace API Claro) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claro-insight-marketplace-api-claro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

The official Claro Brasil API marketplace as an MCP: SIM tenure checks, GSMA KYC match & fill-in, CPF-vs-phone and CPF-vs-address validation, Claro Score credit scoring and facial biometrics lookup — OAuth client_credentials.

## Description
The **official Claro Insight API Marketplace** (claroinsight.com.br) as a single MCP server — Claro Brasil's carrier-grade identity, antifraud and scoring APIs, including the GSMA Open Gateway suite.

### What you can do
- **SIM tenure** — how long a phone number has been active on the Claro network, with the associated plan
- **Valida Telefone** — verify that a CPF is the registered owner of a Claro mobile line
- **Claro Score** — credit score (0–1000) by CPF, built from Claro payment behavior, covering unbanked consumers
- **Valida Endereço 2.0** — antenna-proximity score for whether a CPF/phone really belongs to an address
- **KYC Match (GSMA)** — compare user-supplied phone/ID/name/birthdate against Claro verified records
- **KYC Fill-In (GSMA)** — auto-fill onboarding data (name, CPF, birthdate, address, e-mail) from an authorized MSISDN
- **Face Match** — check whether a CPF has a registered facial biometric in the Claro customer database

### Authentication (from the official per-API code samples)
1. Register an app in the **Claro Insight marketplace** to get a Client ID + Client Secret (free trials with 1.000 requests are offered per API)
2. The MCP mints a token at `POST https://api.claro.com.br/oauth2/v1/token` (`grant_type=client_credentials`, HTTP Basic) and refreshes it automatically
3. The legacy `customers/*` APIs additionally require your marketplace **Customer ID** (X-CustomerID header) — optional credential in this MCP

### Who is this for?
Onboarding and identity-verification flows, fintech/antifraud agents, credit and KYC automation — anyone integrating with Brazil's largest carrier API marketplace.


## Available Tools (7)
- **validate_phone**: Use to catch borrowed or mis-typed phone numbers in onboarding, payments and account recovery. cpf = 11 digits; network_msisdn = country code + number, digits only ("5521987654321"). Requires the optional credential CLARO_CUSTOMER_ID.

Validate whether a CPF and a mobile number belong to the same person (Claro Valida Telefone)
- **kyc_match**: Include every field the user provided — each verified field strengthens the overall verdict, and any failed field is a strong identity-fraud signal; phone_number alone is valid when that is all you have. Use in digital onboarding and account-opening flows. phone_number in E.164 ("+5511999999999"); id_document = CPF digits; birthdate = YYYY-MM-DD. A "not found" style response means the number is not in the Claro base, not a mismatch.

Match user-supplied identity data (phone, ID document, name, birthdate) against Claro verified records — per-field match verdict for onboarding
- **kyc_fill_in**: Use to pre-fill onboarding forms instead of asking the user to type them: raises conversion and cuts identity-fraud risk. Only the phone number is needed. phone_number in E.164 ("+5511999999999"). Tell the user their data comes from their operator records and was legally authorized — LGPD applies.

Auto-fill onboarding registration data (full name, CPF, birthdate, address, e-mail) from a Claro Brasil phone number
- **validate_address**: Use to catch fake or borrowed addresses during onboarding and delivery/credit flows. Send the full combo: cpf, zip_code (8 digits, numbers only), address_number (street number) and network_msisdn (country code + number, digits only). Requires the optional credential CLARO_CUSTOMER_ID.

Validate whether a CPF/phone really belongs to an address — antenna-proximity score (Claro Valida Endereço 2.0)
- **get_credit_score**: Distinctive versus traditional bureaus: it is built from Claro customer payment behavior, so it also scores unbanked people. Use for credit decisions, offer eligibility and risk triage. cpf = 11 digits, numbers only. Requires the optional credential CLARO_CUSTOMER_ID.

Get the Claro Score (0-1000) for a CPF — credit-risk scoring built from Claro payment behavior, covering unbanked consumers too
- **check_face_biometrics**: Use to decide the onboarding path: exists=true lets you run a face comparison against the registered biometric; exists=false means fall back to document verification. CPF is zero-padded to 11 digits automatically. Two useful signals that look like errors but are not: a "customer not found in base" response means the CPF is not in the Claro base at all (inform the user, do not retry), and a forbidden-style response means the user's connection is established on the operator network — which itself confirms the line is on Claro.

Check whether a CPF has a registered facial biometric in the Claro customer database (Face Match exists-check)
- **get_sim_tenure**: Use as a trust signal in onboarding and identity checks: a number with very short tenure is riskier for account opening and credit decisions. phone_number = country code + number, digits only ("5511999999999"). If the response says the number is not in the base, tell the user the line is not a Claro Brasil number rather than treating it as an error.

Check how long a Claro Brasil phone number has been active on the network and which plan the line has


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claro Insight (Marketplace API Claro)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check how long the phone 5511999999999 has been a Claro customer"

**🤖 AI Agent:**
> 📶 **Claro Insight: Tenure 5511999999999**

The tenure check returns the activation period of the line on the Claro network plus the plan associated with it — payload below.

Useful as a trust signal in onboarding: numbers with very short tenure are riskier. Want a KYC match against a name/CPF as well?

---

**👤 You:**
> "Validate that CPF 12345678909 is the owner of the Claro line 5521987654321"

**🤖 AI Agent:**
> ✅ **Valida Telefone: 5521987654321**

The endpoint cross-checks the CPF against the registered owner of the line — verdict in the payload below.

A mismatch is a strong signal of a borrowed or mis-typed number; pair it with validate_address when you also need the address check.

---

**👤 You:**
> "Validate that CPF 12345678909 with name João da Silva and birthdate 1990-01-01 matches Claro records for +5511999999999"

**🤖 AI Agent:**
> ✅ **KYC Match: +5511999999999**

Sent phoneNumber, idDocument, name and birthdate to the GSMA KYC Match endpoint — the response carries a per-field match verdict against Claro's verified records, payload below.

Any field that fails is a strong onboarding fraud signal. Want to auto-fill the rest of the registration with KYC Fill-In?


## ❓ FAQ

**Q: How do I get the Client ID/Secret?**
Register at claroinsight.com.br (Marketplace API Claro) and subscribe to the APIs you need — most offer a free trial with 1.000 requests for 3 months. The marketplace issues a Client ID + Client Secret; this MCP exchanges them at POST https://api.claro.com.br/oauth2/v1/token (grant_type=client_credentials) and refreshes the bearer automatically.

**Q: Which tools need the optional Customer ID?**
Every tool sends your marketplace identifier as the X-CustomerID header — configure the three credentials (Client ID, Client Secret, Customer ID) once at activation and all seven tools work. Phone formats differ: the customers/* APIs (score, phone & address validation) and tenure use digits-only MSISDNs (5511999999999), while the GSMA mobile/v1 endpoints (KYC match & fill-in) use E.164 (+5511999999999). Face Match takes the CPF and zero-pads it automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claro-insight-marketplace-api-claro](https://vinkius.com/ai-agent-connect/claro-insight-marketplace-api-claro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claro Insight (Marketplace API Claro)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claro-insight-marketplace-api-claro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claro Insight (Marketplace API Claro)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claro-insight-marketplace-api-claro": {
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
