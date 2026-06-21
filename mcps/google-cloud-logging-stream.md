# Google Cloud Logging Stream MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-logging-stream)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-cloud-logging-stream-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-cloud-logging-stream-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it queries logs using Google Cloud Logging. That's its only function, and nothing else. Incredible for giving your AI secure observability.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to run scoped queries on Google Cloud Logging for specific resources.**

By strictly scoping access, your AI can safely troubleshoot application errors, analyze traffic spikes, and monitor infrastructure without ever gaining access to sensitive audit trails globally.

### The Superpowers

- **Absolute Containment:** The agent is strictly limited to query specific logs using your precise filter setup.
- **Native Logging Querying:** Supports full Cloud Logging syntax, allowing the AI to filter, parse JSON payloads, and extract insights.
- **Plug & Play Troubleshooting:** Instantly gives your agent the eyes and ears it needs to debug production issues autonomously.


## Available Tools
- **stream_logs**: You can optionally filter them using advanced GCP Logging filter syntax (e.g., severity>=ERROR).

Read and search log entries from the configured Google Cloud Log


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Logging Stream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the last 100 log entries from our configured log stream."

**🤖 AI Agent:**
> I've retrieved the latest 100 entries. They are mostly standard info-level logs, but I noticed a warning around 10:14 AM.

---

**👤 You:**
> "Stream logs filtering only for 'severity>=ERROR'."

**🤖 AI Agent:**
> I found 3 matching error logs. The most recent one indicates a database connection timeout.

---

**👤 You:**
> "Search the logs for the user ID 'user_8819' in the JSON payload."

**🤖 AI Agent:**
> Applying the filter `jsonPayload.userId="user_8819"`, I found the specific event where the user triggered the payment webhook.


## Installation & Usage

To install and use the **Google Cloud Logging Stream** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-logging-stream](https://vinkius.com/mcp/google-cloud-logging-stream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
