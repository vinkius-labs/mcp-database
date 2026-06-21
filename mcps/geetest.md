# Geetest MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geetest)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/geetest-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/geetest-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

The ultimate anti-bot CAPTCHA API — validate users, detect bots, and protect your forms with Geetest v4.

## Description
Connect **Geetest** (极验) CAPTCHA v4 to any AI agent and manage bot protection through natural conversation. Validate CAPTCHAs, monitor risk levels, configure policies, and track validation statistics — all via API.

### What you can do
- **CAPTCHA Validation** — Verify user completion tokens from frontend widgets
- **Risk Assessment** — Evaluate user IP and behavior patterns for bot detection
- **Policy Management** — Configure validation modes, risk thresholds, and IP whitelists
- **Statistics** — Monitor pass/blocked counts and identify attack patterns
- **IP Blocking** — View and manage blocked IP addresses from repeated failures
- **Config Management** — Verify and update CAPTCHA display settings

### How it works
1. Subscribe to this server
2. Enter your Geetest Captcha ID and Private Key
3. Start managing bot protection from Claude, Cursor, or any MCP client

### Who is this for?
- **Security Teams** — Monitor CAPTCHA effectiveness and bot attack patterns
- **Developers** — Validate CAPTCHA responses and configure protection policies
- **Product Managers** — Track validation rates and identify false positives


## Available Tools
- **get_blocked_ips**: Useful for investigating false positives and monitoring attack sources.

Get list of IPs blocked by CAPTCHA system
- **get_captcha_config**: Useful for verifying setup and troubleshooting frontend integration.

Get current CAPTCHA configuration and settings
- **get_validation_stats**: Useful for monitoring bot attack patterns and CAPTCHA effectiveness.

Get CAPTCHA validation statistics
- **set_policy**: Changes take effect immediately.

Configure CAPTCHA policy settings
- **validate_captcha**: Requires lot_number, captcha_output, pass_token, and gen_time from the frontend. Returns whether the captcha passed and risk assessment details.

Validate a Geetest v4 CAPTCHA response
- **validate_with_risk**: Provides more accurate bot detection by analyzing user behavior patterns alongside the CAPTCHA result.

Validate CAPTCHA with additional risk control data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geetest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this CAPTCHA: lot_number=abc123, pass_token=xyz789"

**🤖 AI Agent:**
> ✅ CAPTCHA validation PASSED! Risk level: low. User behavior verified as human.

---

**👤 You:**
> "Show me today's validation statistics."

**🤖 AI Agent:**
> 📊 Today's stats: 1,250 total attempts, 1,180 passed (94.4%), 70 blocked (5.6%). Normal traffic pattern detected.

---

**👤 You:**
> "Show me all blocked IPs from the CAPTCHA system."

**🤖 AI Agent:**
> 🚫 2 IPs currently blocked: 1.2.3.4 (15 failed attempts), 5.6.7.8 (8 failed attempts).


## Installation & Usage

To install and use the **Geetest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geetest](https://vinkius.com/mcp/geetest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
