# Sumsub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sumsub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sumsub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sumsub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automate identity verification (KYC/AML) via Sumsub — create applicants, check verification status, and manage documents directly from any AI agent.

## Description
Connect your **Sumsub** account to any AI agent to streamline your identity verification and compliance workflows through natural conversation.

### What you can do

- **Applicant Management** — Create new applicants for KYC/AML verification levels and retrieve full profile data using unique IDs.
- **Status Tracking** — Monitor the real-time verification status of any applicant to ensure compliance requirements are met.
- **Document Handling** — Upload identity documents (passports, ID cards) directly to an applicant's profile using base64 encoding.
- **WebSDK Integration** — Generate secure access tokens to initialize the Sumsub WebSDK for your end-users seamlessly.

### How it works

1. Subscribe to this server
2. Enter your Sumsub App Token and Secret Key
3. Start managing your compliance and onboarding flows from Claude, Cursor, or any MCP-compatible client

No more manual status checks in the dashboard. Your AI acts as a compliance assistant, handling the technical heavy lifting of the Sumsub API.

### Who is this for?

- **Compliance Officers** — quickly check applicant statuses and verification details without leaving your workspace.
- **Fintech Developers** — test and manage applicant creation and token generation directly from your IDE.
- **Operations Teams** — automate the collection and processing of identity documents for faster onboarding.


## Available Tools
- **add_document**: Upload a document for an applicant
- **create_applicant**: Create a new Sumsub applicant
- **generate_access_token**: Generate WebSDK access token
- **get_applicant_status**: Get applicant verification status
- **get_applicant**: Get applicant data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sumsub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Sumsub applicant for user 'ext_user_99' at the 'basic-kyc' level."

**🤖 AI Agent:**
> I've created the applicant. The Sumsub Applicant ID is '65b2f...a1'. You can now proceed with document uploads or status checks for this user.

---

**👤 You:**
> "Check the verification status for applicant ID 65b2f8e9c1234567890."

**🤖 AI Agent:**
> The applicant '65b2f8e9c1234567890' is currently in the 'pending' state. Sumsub is reviewing the submitted documents.

---

**👤 You:**
> "Generate a WebSDK access token for user 'user_456' at the 'advanced-verification' level."

**🤖 AI Agent:**
> Generated token: 'sb:eyJhbG...'. You can use this token to initialize the Sumsub WebSDK for 'user_456'.


## Installation & Usage

To install and use the **Sumsub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sumsub](https://vinkius.com/mcp/sumsub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
