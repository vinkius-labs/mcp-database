# Onfido MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onfido)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onfido-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onfido-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate identity verification via Onfido — create applicants, manage workflow runs, and retrieve verification reports directly from any AI agent.

## Description
Connect your **Onfido** account to any AI agent to streamline your KYC (Know Your Customer) and identity verification processes through natural conversation.

### What you can do

- **Applicant Management** — Create and manage applicant profiles representing individuals undergoing verification.
- **Workflow Studio Integration** — Start and monitor complex verification workflows (Workflow Runs) to automate multi-step identity checks.
- **Legacy Checks** — Create classic checks for specific report combinations like document verification and facial similarity.
- **Detailed Reporting** — Retrieve comprehensive verification reports, including results and granular breakdowns of identity data.
- **Real-time Notifications** — Register webhooks to receive asynchronous updates on verification statuses directly to your systems.

### How it works

1. Subscribe to this server
2. Enter your Onfido API Token
3. Start managing identity verifications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers** — instantly check the status of an applicant's verification or review report breakdowns without manual dashboard searching.
- **Fintech Developers** — integrate and test identity verification flows directly from the code editor or terminal.
- **Operations Teams** — automate the creation of applicants and trigger verification workflows as part of user onboarding.


## Available Tools
- **create_applicant**: Create a new Onfido applicant
- **create_check**: Create a new Check (Legacy/Classic)
- **create_workflow_run**: Create a new Workflow Run
- **get_report**: Retrieve a Verification Report
- **get_workflow_run**: g., awaiting_input, processing, approved, review, declined).

Retrieve a Workflow Run
- **register_webhook**: Register a new Webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Onfido** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Onfido applicant for John Doe (john.doe@example.com)."

**🤖 AI Agent:**
> I've created the applicant John Doe. The Applicant ID is 'app_12345'. You can now use this ID to start a verification workflow or a check.

---

**👤 You:**
> "Start a verification workflow 'wf_abc' for applicant 'app_12345'."

**🤖 AI Agent:**
> Workflow run 'wr_999' has been started for applicant 'app_12345'. The current status is 'awaiting_input'.

---

**👤 You:**
> "Retrieve the details for report ID 'rep_xyz789'."

**🤖 AI Agent:**
> I've fetched the report 'rep_xyz789'. The result is 'clear' with a breakdown showing document validity and image integrity are confirmed.


## Installation & Usage

To install and use the **Onfido** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onfido](https://vinkius.com/mcp/onfido)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
