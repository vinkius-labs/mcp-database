# Vibrato MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vibrato)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vibrato-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vibrato-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Manage secrets and environment variables securely across your development and deployment pipeline with encrypted vaults.

## Description
Connect your **Vibrato** account to any AI agent to unlock human-like phone interaction capabilities. Vibrato provides a powerful API for programmatically initiating AI-powered calls to handle complex real-world tasks like negotiating cable bills, booking doctor appointments, or inquiring about business hours.

### What you can do

- **AI-Powered Calling** — Start new phone calls by providing a natural language prompt and the target phone number
- **Template-Based Tasks** — Use predefined task templates (e.g., 'Negotiate Comcast Bill') for high-success rate automations
- **Real-time Status Tracking** — Monitor the status of your calls and retrieve live transcripts and final summaries
- **Call Library Management** — List all your previous AI calls and access their detailed recordings and metadata
- **Global Locale Support** — Initiate calls in different languages and locales to reach businesses worldwide

### How it works

1. Subscribe to this server
2. Enter your Vibrato API Key from your account settings at getvibrato.com
3. Start automating your phone tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Personal Productivity** — automate tedious phone calls for bill negotiation and personal scheduling
- **Business Operations** — scale outbound inquiries and customer follow-ups using AI voice agents
- **Developers** — integrate real-time voice automation and calling intelligence into custom applications


## Available Tools
- **create_call_from_template**: g., Negotiate Bill).

Initiate a call using a template
- **create_call**: Pass prompt, phone number, and locale in the JSON body.

Create an AI-powered phone call
- **get_call_status**: Check status of a call
- **list_calls**: List all AI calls
- **list_templates**: List available call templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vibrato** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Call +123456789 to negotiate my internet bill using the 'Telecom Negotiation' template."

**🤖 AI Agent:**
> I've initiated the AI call to negotiate your bill. You can track the progress and see the final outcome here: [View Call Status].

---

**👤 You:**
> "Book a dentist appointment at 'City Dental' (+198765432) for next Tuesday morning."

**🤖 AI Agent:**
> Call started! The AI agent is currently speaking with City Dental to secure your appointment. I'll provide the confirmation details shortly.

---

**👤 You:**
> "Show the transcript for my last call."

**🤖 AI Agent:**
> I've retrieved the transcript. The AI successfully negotiated a $20/month discount on your plan. Here is the full conversation: [View Transcript].


## Installation & Usage

To install and use the **Vibrato** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vibrato](https://vinkius.com/mcp/vibrato)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
