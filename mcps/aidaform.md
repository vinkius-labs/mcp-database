# AidaForm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aidaform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aidaform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aidaform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design beautiful online forms, quizzes, and surveys that convert and collect structured data effortlessly.

## Description
Connect your **AidaForm** account to any AI agent and take full control of your online form builder and automated response management workflows through natural conversation.

### What you can do

- **Form Orchestration** — List and manage your entire high-fidelity form directory programmatically, retrieving detailed metadata and configuration for every survey
- **Response Intelligence** — Programmatically retrieve all submitted responses for specific forms and access complete data for individual submissions in real-time
- **Data Hygiene Management** — Programmatically delete specific responses to maintain high-fidelity database integrity and organizational compliance
- **Insight Discovery** — Access detailed form metadata to coordinate your data collection strategy and monitor active survey statuses directly through your agent
- **Operational Monitoring** — Verify API connectivity and retrieve account-level metadata directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AidaForm dashboard (Settings > API Key)
3. Start orchestrating your data collection from Claude, Cursor, or any MCP client

No more manual logging into form portals to check for new leads or feedback. Your AI acts as your dedicated data coordinator and survey architect.

### Who is this for?

- **Marketing Managers** — instantly retrieve lead responses and monitor survey completion rates using natural language commands
- **HR & Ops Teams** — track recruitment forms and employee feedback without leaving your creative workspace
- **Developers** — integrate high-speed form data and response intelligence into custom workflows through simple AI queries


## Available Tools
- **check_aidaform_status**: Verify connectivity
- **create_form**: Create a form
- **delete_form**: Delete a form
- **delete_response**: Delete a response
- **export_responses**: Export responses
- **get_form_analytics**: Get form analytics
- **get_form**: Get form details
- **get_response**: Get response details
- **list_forms**: List forms
- **list_responses**: List form responses
- **list_workspaces**: List workspaces
- **update_form**: Update a form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AidaForm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my AidaForm account."

**🤖 AI Agent:**
> I've retrieved your form directory. You currently have 5 active forms, including 'Lead Gen v2' (ID: 12345) and 'Customer Satisfaction'. Which one should we check for new responses?

---

**👤 You:**
> "Show the last 3 responses for form 'Lead Gen v2'."

**🤖 AI Agent:**
> Fetching responses... For form 12345, I've identified 3 recent submissions today, including @user1 and @user2. Would you like the high-fidelity detailed data for the most recent one?

---

**👤 You:**
> "Delete response ID '987' from form '12345'."

**🤖 AI Agent:**
> Response orchestrated! I've successfully deleted submission 987 from your specified form. The data hygiene operation is complete and no longer appears in your records. Need any other database actions?


## Installation & Usage

To install and use the **AidaForm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aidaform](https://vinkius.com/mcp/aidaform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
