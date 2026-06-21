# IBAN.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibancom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibancom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibancom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Validate and audit banking codes — identify IBAN and SWIFT via AI.

## Description
Empower your AI agent to orchestrate your entire financial auditing and banking verification workflow with **IBAN.com**, the leading platform for payment data intelligence. By connecting IBAN.com to your agent, you transform complex account verification into a natural conversation. Your agent can instantly verify if an IBAN is valid, audit SWIFT/BIC codes, and retrieve detailed bank metadata without you ever touching a manual validation portal. Whether you are managing international payments or conducting financial due diligence, your agent acts as a real-time banking analyst, ensuring your payment data is always verified and accurate.

### What you can do

- **IBAN Auditing** — Verify if any international bank account number is valid and retrieve detailed bank metadata, including branch and city info.
- **SWIFT Oversight** — Audit SWIFT/BIC codes to maintain a clear view of global routing authenticity.
- **Payment Intelligence** — Calculate IBANs from local account details to assist in international payment setup instantly.
- **Compliance Intelligence** — Validate credit card numbers using the Luhn algorithm to ensure data integrity in your financial records.
- **Usage Monitoring** — Check your API request balance and metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your IBAN.com API Key
3. Start managing your banking intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Managers** — monitor payment data and retrieve verified banking metadata straight from your workflow.
- **Accountants** — verify IBAN codes and audit bank distributions for global invoicing without manual searching.
- **Due Diligence Teams** — perform rapid audits of financial routing data and identify institution markers through natural language.
- **Operations Leads** — automate banking data querying to orchestrate cross-functional global finance teams smoothly.


## Available Tools
- **calculate_iban**: Calculate an IBAN from local account details
- **get_api_balance**: Check remaining API request balance
- **get_bank_details**: Get detailed bank information from an IBAN
- **validate_card_luhn**: Validate a credit card number using the Luhn algorithm
- **validate_iban**: Verify if an IBAN code is valid and retrieve bank metadata
- **validate_swift_bic**: Verify if a SWIFT/BIC code is valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBAN.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the IBAN 'DE12345678901234567890' using IBAN.com."

**🤖 AI Agent:**
> IBAN validated! The code is valid and corresponds to Deutsche Bank in Germany. I've retrieved the branch details and SWIFT code. Would you like to check the BIC status as well?

---

**👤 You:**
> "Check the SWIFT/BIC code 'CHASUS33'."

**🤖 AI Agent:**
> I've verified the SWIFT/BIC code. It is valid and identifies J.P. Morgan Chase Bank in the United States. I can provide the associated bank address and city if you'd like.

---

**👤 You:**
> "Calculate the IBAN for a UK account with number 12345678 and sort code 10-20-30."

**🤖 AI Agent:**
> Calculation complete! The resulting IBAN for those details is identified. I've also retrieved the bank name associated with that sort code. Would you like the direct validation results?


## Installation & Usage

To install and use the **IBAN.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibancom](https://vinkius.com/mcp/ibancom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
