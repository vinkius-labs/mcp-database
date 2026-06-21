# SEON MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seon)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/seon-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/seon-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Prevent online fraud with device fingerprinting, email and phone analysis, and real-time risk scoring for digital transactions.

## Description
Connect your **SEON** account to any AI agent and take full control of your fraud prevention and risk management orchestration through natural conversation. SEON provides a modular and powerful platform for transaction scoring, digital footprinting, and AML compliance, and this integration allows you to retrieve risk metadata, perform real-time checks, and manage blacklists directly from your chat interface.

### What you can do

- **Fraud & Risk Orchestration** — Perform real-time fraud checks on transactions and registrations programmatically to protect your business revenue.
- **Digital Footprint Intelligence** — Retrieve social media and domain metadata for emails, phone numbers, and IP addresses directly from the AI interface.
- **AML & Compliance Control** — Screen users against global sanctions, PEP, and criminal watchlists to ensure regulatory compliance via natural language.
- **Machine Learning & Feedback** — Send feedback labels and manage custom blacklists/whitelists to train your fraud models and ensure they are always synchronized.
- **Operational Monitoring** — Track fraud rules, monitor account statistics, and retrieve transaction metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your SEON Admin API Key from your dashboard settings
3. Start managing your risk operations from Claude, Cursor, or any MCP-compatible client

No more manual background checks or complex fraud rule management. Your AI acts as a dedicated risk analyst or compliance officer.

### Who is this for?

- **Risk Managers** — quickly retrieve digital footprints and monitor transaction scores without switching apps.
- **Compliance Officers** — automate AML screening and track social media profile data via natural conversation.
- **Operations Teams** — streamline the management of custom lists and monitor organizational fraud health directly within the chat.


## Available Tools
- **add_label**: Add a feedback label
- **add_to_list**: ) to a specific blacklist or whitelist.

Add an item to a list
- **aml_screening**: Perform AML screening
- **check_email**: Get email digital footprint
- **check_fraud**: Perform a comprehensive fraud check
- **check_ip**: Get IP risk data
- **check_phone**: Get phone intelligence
- **get_account_info**: Get account details
- **get_transaction**: Get transaction details
- **list_aml_monitors**: List AML monitors
- **list_lists**: List custom blacklists/whitelists
- **list_rules**: List fraud rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEON** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this email for fraud risk: suspicious.user@example.com."

**🤖 AI Agent:**
> I've retrieved the digital footprint. The email has no linked social media accounts and the domain was registered 2 days ago, resulting in a high risk score of 85. Would you like to check the associated IP address?

---

**👤 You:**
> "Run a fraud risk assessment on a new user registration with email and IP analysis."

**🤖 AI Agent:**
> Fraud assessment completed. Overall risk score: 23/100 (Low Risk). Email analysis: user@gmail.com - Registered 4 years ago, active social profiles (LinkedIn, GitHub), data breach count: 1 (minor). Email score: 15/100 (safe). IP analysis: 203.0.113.45 - ISP: Comcast, Location: San Francisco, CA. VPN: No. Tor: No. Proxy: No. IP score: 18/100 (safe). Device fingerprint: Chrome 125, macOS, unique device. Phone: +1-555-0198 - Carrier: AT&T, type: mobile, valid format. Recommendation: APPROVE.

---

**👤 You:**
> "Show me all flagged transactions from the last 24 hours with their risk scores and reasons."

**🤖 AI Agent:**
> 12 flagged transactions in 24 hours. High risk (3): TX-8923 ($2,400, score 89, disposable email + VPN), TX-8934 ($1,800, score 82, velocity abuse - 5 orders in 10 min), TX-8941 ($3,200, score 91, card-country mismatch + new account). Medium risk (5): velocity patterns, mismatched billing/shipping (scores 55-72). Low risk (4): minor flags, first-time buyers (scores 35-48). Auto-blocked: 2 transactions. Manual review queue: 6. False positive rate (last 30 days): 3.2%.


## Installation & Usage

To install and use the **SEON** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seon](https://vinkius.com/mcp/seon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
