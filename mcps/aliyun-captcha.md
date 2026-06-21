# Aliyun CAPTCHA / 阿里云验证码 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aliyun-captcha)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aliyun-captcha-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aliyun-captcha-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Alibaba Cloud's dominant anti-bot service — verify tickets and audit security risk via AI.

## Description
Empower your AI agent to orchestrate your application security and bot protection with **Aliyun CAPTCHA** (验证码 2.0), the premier defense platform by Alibaba Cloud. By connecting Aliyun CAPTCHA to your agent, you transform complex ticket verification, risk assessment, and security diagnostics into a natural conversation. Your agent can instantly validate frontend CAPTCHA results (VerifyParam), provide detailed explanations of verification result codes, and audit your AccessKey configurations without you ever needing to navigate the comprehensive Aliyun Console. Whether you are building a secure login flow or conducting a real-time risk audit, your agent acts as a real-time security coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Verification Orchestration** — Securely validate CAPTCHA verification parameters from end-user interactions.
- **Risk Auditing** — Interpret result codes to identify human users vs suspicious automated activities.
- **Security Discovery** — Verify supported regions, API version compliance, and signature methods.
- **Diagnostic Auditing** — Validate verification parameter formats and Aliyun Request IDs to ensure high-precision checks.
- **System Monitoring** — Monitor API connectivity and gateway status to maintain robust platform defense.

### How it works

1. Subscribe to this server
2. Enter your Aliyun AccessKey ID and AccessKey Secret
3. Start managing your application security through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate risk audits and monitor CAPTCHA delivery health through natural language.
- **Backend Developers** — integrate world-class bot protection and identity verification into your AI-driven routines.
- **DevOps Teams** — audit security configurations and verify regional API connectivity directly from your workspace.
- **Aliyun Power Users** — integrate your existing CAPTCHA workflows into your AI-driven daily routines.


## Available Tools
- **create_captcha_scene**: g., Login, Checkout). Returns a Scene ID for client-side SDK initialization.

Create a new CAPTCHA verification scenario
- **verify_captcha**: Returns verification result (pass/fail).

Verify a CAPTCHA response


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aliyun CAPTCHA / 阿里云验证码** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify this Aliyun CAPTCHA parameter: '{"token":"...", "sig":"..."}'."

**🤖 AI Agent:**
> I've successfully verified the CAPTCHA parameter. The validation result is 'OK', indicating a valid human interaction. The Aliyun Request ID for this check is `88210934-ABCD`. Should I retrieve your AccessKey status?

---

**👤 You:**
> "Explain the verification result code 'VerifyFailed'."

**🤖 AI Agent:**
> The code 'VerifyFailed' indicates that the CAPTCHA challenge was not completed correctly or was identified as suspicious (likely an automated bot). You should deny the associated action or prompt for a different verification method.

---

**👤 You:**
> "Check the status and supported regions for Aliyun CAPTCHA."

**🤖 AI Agent:**
> I've performed a diagnostic check. The Aliyun CAPTCHA gateway is responding normally. Supported regions for this service include Hangzhou, Shanghai, Beijing, and Singapore. Would you like me to verify your specific configuration?


## Installation & Usage

To install and use the **Aliyun CAPTCHA / 阿里云验证码** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aliyun-captcha](https://vinkius.com/mcp/aliyun-captcha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
