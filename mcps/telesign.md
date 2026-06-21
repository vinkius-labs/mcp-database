# TeleSign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telesign)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/telesign-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/telesign-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Verify user identities with phone number intelligence, SMS verification, and risk scoring that prevents fraud at sign-up.

## Description
Connect your **TeleSign** account to any AI agent and manage phone verification and intelligence.

### What you can do

- **SMS Verification** — Send OTP codes via SMS and validate responses
- **Voice Verification** — Deliver codes via automated voice calls
- **Phone Intelligence** — Identify carrier, line type, and location
- **Fraud Scoring** — Calculate risk scores for phone numbers
- **Number Deactivation** — Check if numbers have been deactivated
- **Push Verification** — Send push notification verification
- **Health Check** — Verify API connectivity


## Available Tools
- **check_deactivation**: Check number deactivation
- **check_telesign_status**: Verify API connectivity
- **check_verification**: Check verification status
- **get_phone_id**: Get phone identity
- **get_phone_type**: Get phone type
- **score_phone**: Score phone risk
- **send_push_verification**: Send push verification
- **send_sms**: Send an SMS message
- **send_verification**: Send verification code
- **send_voice_verification**: Send voice verification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TeleSign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a verification code to +14155551234."

**🤖 AI Agent:**
> Verification code sent! Reference ID: ref_8291. The user should receive the code shortly.

---

**👤 You:**
> "Score fraud risk for +14155551234."

**🤖 AI Agent:**
> Risk score for +14155551234: 120/1000 (Low Risk). Carrier: Verizon, Type: Mobile, Location: San Francisco, CA.

---

**👤 You:**
> "Check if +14155551234 has been deactivated."

**🤖 AI Agent:**
> Number +14155551234 is active. Last ported: 2024-03-15 from AT&T to Verizon. No deactivation detected.


## Installation & Usage

To install and use the **TeleSign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telesign](https://vinkius.com/mcp/telesign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
