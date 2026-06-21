# Chuanglan 253 / 创蓝 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chuanglan-253)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Leading cloud communication and KYC platform in China — send ultra-high volume SMS and verify user identities via AI.

## Description
Empower your AI agent to orchestrate your cloud communication and identity verification infrastructure with **Chuanglan 253** (创蓝云智), the premier SMS and KYC provider in China. By connecting Chuanglan to your agent, you transform complex messaging workflows, identity auditing, and phone verification into a natural conversation. Your agent can instantly send standard or variable SMS, retrieve real-time delivery reports, audit account balances, and perform 2-element or 3-element KYC checks without you ever needing to navigate the comprehensive Chuanglan console. Whether you are automating verification codes or conducting security audits on user registrations, your agent acts as a real-time communication assistant, providing accurate and reliable results from a single, unified source.

### What you can do

- **SMS Orchestration** — Send standard, variable, and international SMS messages with full support for delivery reports.
- **KYC Auditing** — Perform real-time identity verification (name/ID) and phone owner checks (name/ID/phone).
- **Growth Monitoring** — Retrieve real-time account balance statistics and monitor service status across all modules.
- **Identity Verification** — Coordinate one-click login checks (Flash Check) to streamline user onboarding.
- **Delivery Insights** — Pull delivery reports and query specific message statuses to ensure communication reliability.

### How it works

1. Subscribe to this server
2. Enter your Chuanglan Account and Password
3. Start managing your communication infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Operations** — automate verification code lifecycles and monitor SMS delivery through natural language queries.
- **Security Teams** — conduct KYC audits and verify user identities directly from your AI-powered workspace.
- **Developers** — integrate a massive library of communication and identity APIs into your AI-driven daily routines.
- **Chuanglan Power Users** — integrate your existing communication workflows into your AI-driven daily routines.


## Available Tools (9)
- **flash_check**: One-click login check
- **get_balance**: Check account balance
- **pull_sms_reports**: Pull delivery reports
- **query_sms_status**: Query SMS delivery status
- **send_intl_sms**: Send international SMS
- **send_sms**: Send a standard SMS
- **send_variable_sms**: Send variable SMS
- **verify_identity**: Verify identity (2-element)
- **verify_phone**: Verify phone owner (3-element)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chuanglan 253 / 创蓝** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a verification SMS to '13800138000' with text 'Your code is 8821'."

**🤖 AI Agent:**
> I've successfully sent the verification SMS. The message ID is `ch_88210934`. I'll monitor the delivery status and let you know if there are any issues.

---

**👤 You:**
> "Verify identity for 'Zhang San' with ID '110101199001011234'."

**🤖 AI Agent:**
> I've performed the identity verification. The name and ID number provided match the official records. The verification status is 'Success'.

---

**👤 You:**
> "What is my current SMS credit balance?"

**🤖 AI Agent:**
> Your current Chuanglan account balance is 15,240 credits. This should be sufficient for your upcoming promotional campaign. Would you like me to alert you if it drops below 1,000?


## ❓ FAQ

**Q: How do I find my Chuanglan Account and Password?**
Log in to the [Chuanglan Developer Portal](https://open.253.com/), navigate to the 'Application Management' or 'API Settings' section, and you will find your unique Account (username) and Password/Key for integration.

**Q: What is Variable SMS?**
Variable SMS allows you to send template-based messages where specific placeholders (like names or codes) are replaced with different values for each recipient in a single API call.

**Q: Does this work for international numbers?**
Yes! Use the `send_intl_sms` tool to reach users globally. Ensure you provide the phone number with the correct international country code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chuanglan-253](https://vinkius.com/mcp/chuanglan-253)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chuanglan 253 / 创蓝** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chuanglan-253` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chuanglan 253 / 创蓝** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chuanglan-253": {
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
