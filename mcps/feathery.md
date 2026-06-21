# Feathery MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feathery)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feathery-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feathery-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Automate forms and user workflows via Feathery — manage users, retrieve form data, and monitor connector logs directly through your AI agent.

## Description
Connect your **Feathery.io** account to any AI agent and take full control of your form automation and user data management through natural conversation.

### What you can do

- **User Orchestration** — List all users in your environment and fetch detailed profiles including submission history natively
- **Submission Intelligence** — Retrieve granular field data submitted by specific users across all your automated forms flawlessly
- **Session Monitoring** — Query current form sessions to understand user progress and friction points in real-time
- **Connector Auditing** — List API connector logs to verify data synchronization and troubleshoot integration errors synchronously
- **Form Management** — List all active forms and retrieve structural details and metadata directly from the cloud
- **Workflow Tracking** — Inspect automated workflows and their execution status to ensure seamless user journeys
- **Identity Context** — Verify your API token user profile and account information through the agent flawlessly

### How it works

1. Subscribe to this server
2. Enter your Feathery API Key (found in Settings > API)
3. Start managing your forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Operations** — monitor user form progress and troubleshoot submission errors without leaving your chat
- **Customer Success Teams** — quickly look up user-submitted data to personalize support interactions
- **Marketing Engineers** — audit API connector health and verify lead data flow directly from your AI-powered workflow


## Available Tools
- **get_account_info**: Get Feathery account details
- **get_form_details**: Get details for a specific form
- **get_form_session**: Retrieve the current state/session of a specific form for a user
- **get_me**: Get current API token identity info
- **get_user_data**: Get all field values submitted by a specific user across forms
- **get_workflow_details**: Get details for a specific workflow
- **list_connector_logs**: List recent API connector error logs for a specific form
- **list_environments**: List available Feathery environments
- **list_forms**: List all forms in your Feathery account
- **list_users**: List all users in your Feathery environment
- **list_workflows**: List all automated workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feathery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my account."

**🤖 AI Agent:**
> I've retrieved your forms. You have 'User Onboarding' (ID: form_123), 'Customer Feedback' (ID: form_456), and 'Lead Gen' (ID: form_789) currently active. Which one should I inspect?

---

**👤 You:**
> "Show me the data submitted by user user_99."

**🤖 AI Agent:**
> Fetching data for user_99... They submitted 'John Doe', 'john@example.com', and selected 'Premium Plan' in the onboarding form. Would you like to see their full session history?

---

**👤 You:**
> "Check if there are any connector errors for the Onboarding form."

**🤖 AI Agent:**
> Inspecting connector logs... I found one error for form_123: 'Klaviyo API rejected email format'. All other syncs were successful. Shall I retrieve the user ID associated with this error?


## Installation & Usage

To install and use the **Feathery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feathery](https://vinkius.com/mcp/feathery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
