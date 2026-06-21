# Rong360 Open API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rong360-open-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rong360-open-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rong360-open-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Bring high-level financial risk assessment and identity KYC directly to your agent. Evaluate credit scores and verify names.

## Description
Connect your AI backend directly to **Rong360** (融360), a massive financial big-data hub in China. With this MCP server, your LLMs can execute deep background checks, calculate credit risk, and perform facial-KYC without implementing convoluted RSA algorithms manually.

### What you can do

- **Identity Verification** — Check if an ID number matches the provided Real Name directly with authorities
- **Credit Scoring** — Evaluate consumer loaning scores to identify defaulting behaviors instantly
- **Carrier Validation** — Confirm if a given phone number has been officially registered under the user's name

### How it works

1. Subscribe to this server
2. Insert your **App ID** and your **RSA Private Key** from the [Rong360 Open Platform](https://open.rong360.com/)
3. Start verifying consumers dynamically from the MCP console directly

### Who is this for?

- **Fintech Underwriters** — Allow agents to automatically process preliminary credit evaluations before humans review loans
- **P2P Marketplaces** — Detect scammers by verifying carrier information and matching IDs to face scans automatically
- **Security Teams** — Build robust AI vetting workflows prior to onboarding high-value accounts


## Available Tools
- **check_credit_score**: Generate a big data credit score profile
- **detect_face**: Perform facial recognition matching against a government ID
- **validate_mobile_number**: Validate carrier ownership of a mobile phone
- **verify_identity**: Verify a national ID card and real name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rong360 Open API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the identity for the name 'Lu Han', ID Number 1101051990XXXXXXXX."

**🤖 AI Agent:**
> I've checked the KYC registry. The real name matches the ID card number perfectly.

---

**👤 You:**
> "Generate a credit score report for phone 13912345678 and ID 310115XXXX."

**🤖 AI Agent:**
> The Rong360 credit system returns a score of 620. No loan defaulting history was detected, but multiple micro-loan inquiries were made in the last 30 days.


## Installation & Usage

To install and use the **Rong360 Open API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rong360-open-api](https://vinkius.com/mcp/rong360-open-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
