# EU VAT Validator (VIES) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/eu-vat-validator-vies)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Official EU VIES VAT validation for all 27 member states: instant validity checks, registered company name and address, trader-match scoring, batch checks and service-status monitoring — zero auth.

## Description
The **official EU VIES (VAT Information Exchange System)** as a single MCP server — the European Commission's own system for validating VAT identification numbers, made agent-ready.

### What you can do
- **Validate any EU VAT number** against the live Commission registry: valid/invalid, registered trading name and full address
- **Trader-match scoring** — approximate-match breakdown (name, street, postal code, city) with 1/2/3 scores for KYC and intra-EU B2B invoicing
- **Prefixed convenience checks** — paste "PT501964843" or "IE6388047V" exactly as written; country auto-detected (GR→EL, UK→XI)
- **Small batches** — validate up to 5 counterparties in one call, mixed member states
- **Normalize messy input** — offline cleanup of CRM/invoice strings with official per-country format patterns
- **Service monitoring** — live availability of each member state's VAT system (some go offline for maintenance)
- **VAT rates reference** — standard and reduced rates for all member states for pricing and market-entry decisions

### Why VIES and not a scraper
VIES is operated by the European Commission and is the *only* legally recognized source for intra-EU VAT verification. An agent that can check a counterparty's VAT number in real time can support cross-border invoicing, onboarding and compliance workflows with authoritative data — no API key, no registration.

### Typical workflows
- Verify a client's VAT before issuing a zero-rated intra-EU invoice
- KYC: confirm the company name on file matches the VAT registration
- Batch-check a CRM import of EU customers
- Compare VAT rates when pricing a product launch across EU markets


## Available Tools (8)
- **validate_vat_batch**: Pass a JSON array of VAT numbers, each WITH its country prefix, e.g. '["PT501964843","IE6388047V","DE123456789"]'. Each entry is checked individually against VIES and returned with its own validity, name and address. For single lookups prefer validate_vat.

Validate up to 5 EU VAT numbers in one call — mixed member states allowed
- **validate_vat_details**: Use for KYC/counterparty verification when you need to confirm the customer details actually match the VAT registration — e.g. before zero-rating an intra-EU B2B supply. Note: several member states (BE, EL and others) do not return trader data; score 3 means "no data available", not a mismatch.

Full VIES validation with trader-match breakdown: company name, street, postal code, city and approximate-match scores
- **validate_vat_prefixed**: Spaces, dashes and dots are ignored. GR is mapped to EL (Greece) and UK to XI (Northern Ireland). Use when the input comes from free text, invoices or CRM records where the prefix is embedded.

Validate a VAT number written WITH its country prefix (e.g. "PT501964843", "DE123456789") — country auto-detected
- **normalize_vat**: Returns the normalized number ready for validate_vat / validate_vat_prefixed. This does NOT confirm the number is registered — always follow with a VIES check.

Clean and structurally validate a raw VAT string: strips spaces/punctuation, fixes prefixes and checks the member-state format — no API call
- **check_vies_service_status**: IMPORTANT: when a country shows Unavailable (e.g. BE or EL are periodically offline for maintenance), VIES cannot confirm numbers from that state and validation must be retried later — invoicing decisions should not rely on an unverifiable check. Also shows whether the VIES on the Web (VoW) service itself is up.

Live availability of the VIES validation service for every EU member state
- **list_member_states**: g. PT = 9 digits, NL = 9 digits + B + 2, IE = 7 digits + 1-2 chars) and a real example. Use it to pre-format numbers or to explain a validation failure caused by wrong format. Greece is "EL" (not GR) and Northern Ireland is "XI" (post-Brexit protocol).

Reference table of EU member states for VIES: country codes, official VAT format patterns and examples
- **get_vat_rates**: Use when pricing products for an EU market launch or comparing tax burden across member states. Rates are indicative and change occasionally — for legal decisions always confirm with the national tax authority (and note that VIES validates NUMBERS, not rates).

Reference: current standard and reduced VAT rates for all EU member states (for pricing and market-entry decisions)
- **validate_vat**: Required: country_code (2-letter member state: AT BE BG CY CZ DE DK EE EL ES FI FR HR HU IE IT LT LU LV MT NL PL PT RO SE SI SK XI — Greece is EL, Northern Ireland is XI) and vat_number (digits/characters WITHOUT the country prefix). A valid result includes the registered trading name and address — use it to verify a counterparty before invoicing cross-border. For the full company-match breakdown use validate_vat_details.

Validate an EU VAT number against the official VIES system of any member state — returns validity, registered company name and address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU VAT Validator (VIES)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the VAT number IE6388047V valid? Who is it registered to?"

**🤖 AI Agent:**
> ✅ **IE6388047V is VALID**

- Registered to: **GOOGLE IRELAND LIMITED**
- Address: 3RD FLOOR, GORDON HOUSE, BARROW STREET, DUBLIN 4
- Checked against the official EU VIES registry just now

You can invoice this counterparty intra-EU (B2B, reverse charge). If you want, I can also confirm the name/address match against your records (validate_vat_details).

---

**👤 You:**
> "Check these 3 customers from my CRM before I invoice them: PT 501-964 843, DE 129-274-202, BE 0123.456.789"

**🤖 AI Agent:**
> 📋 **Batch check: 2/3 valid**

| Input | Result |
|---|---|
| PT501964843 | ✅ VALID — name and address returned |
| DE129274202 | ⚠️ Valid format, INVALID in registry — re-confirm with the client |
| BE0123456789 | ⚠️ Belgium's VAT service is currently **Unavailable** in VIES — retry in a few hours before invoicing |

Recommendation: invoice only the verified one for now; I can retry Belgium later (check_vies_service_status).

---

**👤 You:**
> "I'm pricing a SaaS product for Germany, France and Portugal — what VAT rates apply?"

**🤖 AI Agent:**
> 💶 **VAT rates for digital services (SaaS)**

- 🇩🇪 Germany: **19%** standard (reduced 7% does not apply to SaaS)
- 🇫🇷 France: **20%** standard
- 🇵🇹 Portugal: **23%** standard (Azores/Madeira have lower regional rates)

Reminder: for B2B sales of digital services across borders, the reverse charge applies — collect the client's VAT number (I can validate it live with validate_vat) and charge 0% intra-EU.


## ❓ FAQ

**Q: Do I need an API key or registration to use this MCP?**
No. VIES is a free public service of the European Commission — every tool in this MCP works without any authentication. The batch tool is limited to 5 numbers per call out of respect for fair use.

**Q: Why do some valid VAT numbers return no company name or address?**
Member states decide how much data they share through VIES. Belgium, Greece and others return validity only (match score 3 = 'no data returned'). The number is still legally valid — only the trader data is withheld. Use the matchScore legend in validate_vat_details to interpret results correctly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/eu-vat-validator-vies](https://vinkius.com/ai-agent-connect/eu-vat-validator-vies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU VAT Validator (VIES)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-vat-validator-vies` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU VAT Validator (VIES)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-vat-validator-vies": {
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
