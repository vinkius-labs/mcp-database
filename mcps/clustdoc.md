# Clustdoc MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clustdoc)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clustdoc-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clustdoc-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage client onboarding and workflows via Clustdoc — track dossiers, monitor applications, and automate invitations directly from any AI agent.

## Description
Connect your **Clustdoc** account to any AI agent and take full control of your client onboarding and document collection through natural conversation. Streamline how you manage complex applications and workflows natively.

### What you can do

- **Template Oversight** — List and retrieve details for all onboarding workflow templates configured in your account natively
- **Dossier Intelligence** — Access and monitor individual client applications (dossiers) and their current progress flawlessly
- **Application Lifecycle** — Launch new onboarding sessions for clients using pre-defined templates securely
- **Invitation Logistics** — Trigger automated portal invitation emails to clients directly from your chat interface flawlessly
- **Team Management** — List all teams and members within your Clustdoc account to manage access flawlessly
- **integrated Visibility** — Retrieve detailed application metadata including status and contact information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clustdoc API Token (obtained from Team Settings > Developer > API)
3. Start managing your client onboarding from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Onboarding Managers** — monitor application volumes and completion rates using natural language
- **Legal & Compliance** — audit document collection progress and dossier statuses without opening the dashboard
- **Customer Success** — quickly look up client application details and trigger invitations straight from their chat interface
- **Ops Teams** — verify workflow configurations and monitor team member activity


## Available Tools
- **launch_new_onboarding**: Launch a new onboarding application for a client
- **get_application_status_details**: Get detailed status and progress for a specific client dossier
- **get_my_clustdoc_profile**: Retrieve information about the authenticated user
- **get_workflow_configuration**: Get detailed configuration for a specific onboarding template
- **list_client_dossiers**: List all active and completed client applications (dossiers)
- **list_clustdoc_teams**: List all teams and members in the Clustdoc account
- **list_onboarding_templates**: List all onboarding workflow templates
- **send_onboarding_invitation**: Send the portal invitation email to the client for a specific dossier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clustdoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active client dossiers in Clustdoc."

**🤖 AI Agent:**
> Retrieving active dossiers... I found 5 applications in progress: 'Acme Corp' (80% complete), 'TechFlow Inc' (45% complete), and 3 others. Would you like to see what's missing for Acme?

---

**👤 You:**
> "Launch a new 'Standard Business Onboarding' for john@example.com."

**🤖 AI Agent:**
> Launching onboarding session... I've created a new dossier for John Doe using the requested template. I can now send the invitation email to his address.

---

**👤 You:**
> "What is the status of the dossier for 'TechFlow Inc'?"

**🤖 AI Agent:**
> Checking status for TechFlow Inc... The dossier is 45% complete. The client has uploaded their business license but we are still waiting for the signed contract and ID proof.


## Installation & Usage

To install and use the **Clustdoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clustdoc](https://vinkius.com/mcp/clustdoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
