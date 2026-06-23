# Tencent CAPTCHA / 腾讯云防水墙 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-captcha)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Tencent's dominant anti-bot and CAPTCHA service — verify tickets and audit risk levels via AI.

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


## Available Tools (2)
- **get_captcha_app_info**: Get CAPTCHA application configuration
- **verify_captcha**: Returns verification result with evil level score. CaptchaType is fixed to 9 (slide).

Verify a CAPTCHA ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent CAPTCHA / 腾讯云防水墙** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify this CAPTCHA ticket: 't0...ABCD' with randstr 'xyz123' from IP '1.2.3.4'."

**🤖 AI Agent:**
> I've successfully verified the CAPTCHA result. The ticket has passed validation with an 'EvilLevel' of 5, indicating a low-risk human user. Should I retrieve the full details for your CaptchaAppId?

---

**👤 You:**
> "What does an EvilLevel of 85 mean?"

**🤖 AI Agent:**
> An EvilLevel of 85 is classified as 'High Risk'. This indicates a very high probability that the interaction originated from a malicious bot or a fraudulent automation script. I recommend blocking this request or requiring additional authentication.

---

**👤 You:**
> "Show me the configuration and status of my Tencent CAPTCHA project."

**🤖 AI Agent:**
> I've retrieved your project overview. Your CaptchaAppId is correctly registered, and the API gateway is responding normally in the 'ap-guangzhou' region. Would you like me to check if your AppSecretKey is also properly configured for verification calls?


## ❓ FAQ

**Q: How do I find my Tencent Cloud SecretId and SecretKey?**
Log in to the [Tencent Cloud Console](https://console.cloud.tencent.com/), navigate to [Access Management] -> [API Key Management] to find or generate your unique SecretId and SecretKey.

**Q: Where do I get the CaptchaAppId and AppSecretKey?**
Navigate to the [Tencent CAPTCHA (防水墙) Console](https://console.cloud.tencent.com/captcha), select your CAPTCHA application, and you will find these identifiers in the application overview or basic information section.

**Q: What is the 'EvilLevel' metric?**
EvilLevel is a risk score (0-100) provided by Tencent Cloud to identify suspicious activity. A higher value indicates a higher probability that the user is a malicious bot or part of a fraudulent attack.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-captcha](https://vinkius.com/mcp/tencent-captcha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent CAPTCHA / 腾讯云防水墙** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tencent-captcha` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent CAPTCHA / 腾讯云防水墙** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-captcha": {
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
