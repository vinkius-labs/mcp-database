# Aptabase (Mobile Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aptabase-mobile-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aptabase-mobile-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aptabase-mobile-analytics-mcp)
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


## Installation & Usage

To install and use the **Aptabase (Mobile Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aptabase-mobile-analytics](https://vinkius.com/mcp/aptabase-mobile-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
