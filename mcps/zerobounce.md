# ZeroBounce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zerobounce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zerobounce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zerobounce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Validate email addresses, check activity data, and improve deliverability using ZeroBounce's real-time verification and AI scoring tools.

## Description
Connect **ZeroBounce** to your AI agent to ensure your email lists are clean, active, and ready for high-performance campaigns. This server provides direct access to industry-leading email verification and deliverability tools.

### What you can do

- **Real-Time Validation** — Instantly check if a single email address is valid, invalid, or a catch-all to protect your sender reputation.
- **Batch Processing** — Validate up to 100 email addresses in a single request for efficient list cleaning.
- **Activity Tracking** — Retrieve activity data to see if an email has been active within the last 30 to 365 days.
- **AI Scoring** — Use the `score_file` tool to receive a quality score (0-100) for email addresses, identifying high-value leads.
- **Credit Management** — Monitor your account balance in real-time to ensure uninterrupted service.

### How it works

1. Subscribe to this server
2. Enter your ZeroBounce API Key
3. Start validating emails and checking deliverability metrics directly from your AI client

### Who is this for?

- **Marketing Teams** — reduce bounce rates and improve campaign ROI by cleaning lists before sending.
- **Sales Professionals** — verify lead contact information in real-time during the prospecting phase.
- **Developers** — integrate email verification into signup flows to prevent fake account creation.


## Available Tools
- **get_activity**: Check email activity data
- **get_credits**: Get remaining ZeroBounce credits
- **score_file**: AI Scoring for a file of emails
- **validate_batch**: Validate a batch of emails
- **validate_email**: Validate a single email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZeroBounce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my remaining ZeroBounce credits."

**🤖 AI Agent:**
> You currently have 12,450 credits remaining in your ZeroBounce account.

---

**👤 You:**
> "Validate the email address 'john.doe@example.com'."

**🤖 AI Agent:**
> The email 'john.doe@example.com' is valid. It is not a disposable address and has a low risk score.

---

**👤 You:**
> "Check if 'marketing@business.com' has been active in the last 90 days."

**🤖 AI Agent:**
> I've checked the activity data. The email 'marketing@business.com' has been active within the last 90 days.


## Installation & Usage

To install and use the **ZeroBounce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerobounce](https://vinkius.com/mcp/zerobounce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
