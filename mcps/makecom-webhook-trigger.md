# Make.com Webhook Trigger MCP Server

This MCP does exactly one thing: it sends JSON payloads to Make.com Webhooks. That's its only function. Incredible for connecting AI agents to thousands of visual automation workflows instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/makecom-webhook-trigger)

## Overview
**Category:** growth-engine
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Make.com Webhook Trigger** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makecom-webhook-trigger](https://vinkius.com/mcp/makecom-webhook-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
