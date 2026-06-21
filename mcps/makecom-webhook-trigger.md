# Make.com Webhook Trigger MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/makecom-webhook-trigger)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/makecom-webhook-trigger-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/makecom-webhook-trigger-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

This MCP does exactly one thing: it sends JSON payloads to Make.com Webhooks. That's its only function. Incredible for connecting AI agents to thousands of visual automation workflows instantly.

## Description
We refused to build thousands of individual MCP integrations for every SaaS app in the world. Instead, this MCP server provides a universal, zero-trust bridge to Make.com (formerly Integromat): **just triggering a Custom Webhook.**

Your AI agent gains the immediate, zero-friction ability to kick off complex workflows—like generating contracts, issuing invoices, or adding contacts to CRMs—by simply dumping a structured JSON payload into a Make.com scenario.

### The Superpowers

- **The Ultimate Joker Card:** Why code a custom API integration when you can just build a scenario in Make? The agent sends the data, and Make does the visual routing to over 5,000+ apps.
- **Zero-Bloat Integration:** No massive SDKs. It uses a direct `POST` fetch to your specific Make Custom Webhook URL. You just provide the URL and the AI provides the JSON.
- **Absolute Containment:** Because this is strictly a sending tool (Push only), the agent cannot read your Make.com account, cannot edit your scenarios, and cannot access other webhooks. It is a secure, one-way trigger.


## Available Tools
- **trigger_make_webhook**: com scenario. Provide the data you want to send in the "payloadJson" parameter as a valid JSON string. The Make scenario will receive this data and process it.

Send a JSON payload to a Make.com (Integromat) Custom Webhook to trigger an automation scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Make.com Webhook Trigger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger the Make webhook with a JSON payload containing the customer's name and email to start the onboarding flow."

**🤖 AI Agent:**
> I've successfully triggered the Make.com webhook with the requested payload.


## Installation & Usage

To install and use the **Make.com Webhook Trigger** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makecom-webhook-trigger](https://vinkius.com/mcp/makecom-webhook-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
