# Tencent CAPTCHA / 腾讯云防水墙 MCP Server

Tencent's dominant anti-bot and CAPTCHA service — verify tickets and audit risk levels via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-captcha)

## Overview
**Category:** industry-titans
**Tools Count:** 2

## Description
Empower your AI agent to orchestrate your application security and bot protection with **Tencent CAPTCHA** (防水墙), the dominant anti-fraud and CAPTCHA platform in China. By connecting Tencent CAPTCHA to your agent, you transform complex ticket verification, risk level auditing, and security diagnostics into a natural conversation. Your agent can instantly validate frontend CAPTCHA results (ticket and randstr), provide detailed explanations of suspicious 'EvilLevel' numeric values, and audit your AppId configurations without you ever needing to navigate the comprehensive Tencent Cloud Console. Whether you are building a secure registration flow or conducting a real-time risk assessment, your agent acts as a real-time security coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Verification Orchestration** — Securely validate CAPTCHA tickets and random strings from end-user interactions.
- **Risk Level Auditing** — Interpret 'EvilLevel' metrics to identify human users vs suspicious bot activities.
- **Security Discovery** — Verify AppId information, supported regions, and API version compliance.
- **Diagnostic Auditing** — Validate user IP formats and ticket strings to ensure high-precision security checks.
- **System Monitoring** — Monitor API connectivity and gateway status to maintain robust platform protection.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId, SecretKey, CaptchaAppId, and AppSecretKey
3. Start managing your application security through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate risk assessments and monitor CAPTCHA delivery health through natural language.
- **Backend Developers** — integrate world-class bot protection and identity verification into your AI-driven routines.
- **DevOps Teams** — audit security configurations and verify API connectivity directly from your workspace.
- **Tencent Cloud Power Users** — integrate your existing CAPTCHA workflows into your AI-driven daily routines.


## Available Tools
- **get_captcha_app_info**: Get CAPTCHA application configuration
- **verify_captcha**: Returns verification result with evil level score. CaptchaType is fixed to 9 (slide).

Verify a CAPTCHA ticket


## Installation & Usage

To install and use the **Tencent CAPTCHA / 腾讯云防水墙** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-captcha](https://vinkius.com/mcp/tencent-captcha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
