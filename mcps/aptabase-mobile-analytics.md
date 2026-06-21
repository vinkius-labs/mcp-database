# Aptabase (Mobile Analytics) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aptabase-mobile-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send telemetry and custom events to Aptabase directly from your AI agent to track app usage and performance.

## Description
Connect your **Aptabase** account to any AI agent to streamline your mobile and desktop analytics workflow. Aptabase is a privacy-first, open-source alternative to Google Analytics and Firebase.

### What you can do

- **Event Tracking** — Send custom events like `app_started`, `purchase_completed`, or `button_clicked` with specific properties.
- **System Metadata** — Include detailed system information such as OS name, version, app version, and locale for precise segmentation.
- **Privacy-First Analytics** — Leverage Aptabase's privacy-centric approach to collect data without compromising user trust.
- **Custom Properties** — Attach flat JSON objects to your events to capture granular user behavior and business metrics.

### How it works

1. Subscribe to this server
2. Enter your Aptabase App Key
3. Start sending telemetry data from your AI agent or development environment

### Who is this for?

- **Mobile Developers** — quickly test event triggers and telemetry payloads during development without manual SDK implementation.
- **Product Managers** — simulate and verify analytics events for new features directly through conversation.
- **QA Engineers** — automate the validation of analytics tracking across different OS versions and locales.


## Available Tools
- **send_event**: Processes events asynchronously.

Send an event to Aptabase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aptabase (Mobile Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an 'app_launch' event for my iOS app version 1.0.1."

**🤖 AI Agent:**
> I've successfully sent the 'app_launch' event to Aptabase for iOS 17.0 (en-US) using version 1.0.1 of your application.

---

**👤 You:**
> "Track a 'purchase_completed' event with properties for 'plan: pro' and 'amount: 19.99'."

**🤖 AI Agent:**
> The 'purchase_completed' event has been dispatched with your custom properties (plan: pro, amount: 19.99) to your Aptabase project.

---

**👤 You:**
> "Log a telemetry event for a Windows desktop app version 2.4.0 named 'sync_started'."

**🤖 AI Agent:**
> I've recorded the 'sync_started' event for Windows 11 (app version 2.4.0) in your Aptabase analytics dashboard.


## ❓ FAQ

**Q: Can I send custom metadata with my events?**
Yes! Use the `props` field in the `send_event` tool to provide a JSON object with key-value pairs representing your custom properties.

**Q: Is it possible to track the specific OS version?**
Absolutely. The `send_event` tool requires `osName` and `osVersion` parameters to ensure your telemetry is correctly segmented in the Aptabase dashboard.

**Q: Can I use this for self-hosted Aptabase instances?**
Yes, you can optionally provide a `baseUrl` in the configuration to point the MCP server to your own self-hosted Aptabase instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aptabase-mobile-analytics](https://vinkius.com/mcp/aptabase-mobile-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aptabase (Mobile Analytics)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aptabase-mobile-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aptabase (Mobile Analytics)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aptabase-mobile-analytics": {
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
