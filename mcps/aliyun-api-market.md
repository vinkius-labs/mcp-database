# Aliyun API Market / 阿里云云市场 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aliyun-api-market)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's largest API marketplace — access thousands of 3rd-party OCR, SMS, and data services via AI.

## Description
Empower your AI agent to orchestrate thousands of professional data services with the **Aliyun API Market** (阿里云云市场), the premier gateway for third-party cloud capabilities in China. By connecting the Aliyun Market to your agent, you transform complex API integrations for OCR, SMS delivery, identity verification, and logistics tracking into a natural conversation. Your agent can instantly recognize text from images, send verification codes, lookup geographic data, and audit shipment statuses without you ever needing to write custom integration code for each provider. Whether you are conducting compliance audits or managing mobile operations, your agent acts as a unified interface for the entire Aliyun API ecosystem, providing accurate and reliable results from a single, authorized source.

### What you can do

- **API Orchestration** — Call any Aliyun Market API using your unified AppCode for fast and secure access.
- **Visual Intelligence** — Extract structured text from images using professional OCR services for documents and IDs.
- **Communication Control** — Send SMS messages and manage mobile recharges directly through authorized market providers.
- **Identity Verification** — Verify ID cards and bank card metadata against official records for KYC compliance.
- **Logistics Auditing** — Track express shipments and retrieve real-time delivery histories from multiple carriers.

### How it works

1. Subscribe to this server
2. Enter your Aliyun AppCode from the Aliyun Console
3. Start querying thousands of data services through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Back-end Developers** — prototype and integrate third-party data services into your AI-driven daily routines.
- **Compliance Officers** — automate KYC and identity verification checks through natural language queries.
- **Logistics Managers** — monitor delivery statuses and audit carrier performance directly from your AI-powered workspace.
- **Aliyun Market Power Users** — integrate your existing data service subscriptions into your AI-driven daily routines.


## Available Tools
- **bank_card_check**: Check bank card information
- **call_market_api**: Call any Aliyun Market API
- **express_tracking**: Track express shipment
- **ip_lookup**: Lookup IP address location
- **mobile_recharge**: Perform mobile phone recharge
- **ocr_general**: Recognize text from image (General)
- **query_weather**: Query weather by city
- **send_sms**: Send SMS via market provider
- **verify_id_card**: Verify ID card and name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aliyun API Market / 阿里云云市场** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recognize the text from this invoice image: [URL]."

**🤖 AI Agent:**
> I've processed the image using the Aliyun Market OCR service. The invoice total is 1,250.00 CNY, dated Oct 27, 2023. I've extracted all line items into a structured format for you.

---

**👤 You:**
> "Verify that ID card '110101...' belongs to 'Zhang San'."

**🤖 AI Agent:**
> I've performed the identity check. The name and ID card number match the official records. The verification status is 'Match'.

---

**👤 You:**
> "Track my express package with number 'YT88210934'."

**🤖 AI Agent:**
> I've retrieved the tracking history. Your package from YuanTong Express is currently in Shanghai and was processed at the sorting center at 10:30 AM today. It is expected to arrive tomorrow.


## ❓ FAQ

**Q: How do I find my Aliyun AppCode?**
Log in to the [Aliyun Console](https://market.console.aliyun.com/), go to 'Purchased Services', and select an API subscription. Your unique AppCode will be displayed in the API details or application management section.

**Q: Do I need to subscribe to each API individually?**
Yes. Before calling a specific API via this server, you must have an active subscription (often with a free tier) for that service in the Aliyun Market to use your AppCode.

**Q: Can I use this for any provider on the market?**
This server uses the standard `Authorization: APPCODE` header, which is supported by the vast majority of APIs on the Aliyun Cloud Market. Some high-security official services might require AK/SK signatures which are not the primary focus of this connector.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aliyun-api-market](https://vinkius.com/mcp/aliyun-api-market)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aliyun API Market / 阿里云云市场** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aliyun-api-market` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aliyun API Market / 阿里云云市场** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aliyun-api-market": {
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
