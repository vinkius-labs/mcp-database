# Yousign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yousign-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yousign-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yousign-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Secure electronic signatures for documents and contracts with AI using Yousign V3.

## Description
Connect your **Yousign** account to any AI agent to automate your electronic signature workflows and contract management through natural conversation.

### What you can do

- **Request Management** — Create and manage electronic signature requests for multiple documents and signers.
- **Signer Customization** — Add signers with customizable signature levels and authentication modes (OTP, no-OTP).
- **Real-time Monitoring** — Track signature request status in real-time and automate the activation/sending process.
- **Compliance & Auditing** — Download signed documents and comprehensive audit trails for full legal compliance.

### How it works

1. Subscribe to this server
2. Enter your Yousign API Key from your account settings
3. Start managing your e-signatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Teams** — automate the sending of employment contracts and onboarding documents.
- **Legal Departments** — manage contract lifecycles and ensure all agreements are legally binding.
- **Sales Operations** — accelerate deal closures by automating the signature process for sales agreements.


## Available Tools
- **activate_signature_request**: Send for signature
- **add_document_to_request**: Note: In this version, pass metadata info.

Upload PDF to sign
- **add_signer_to_request**: Define who signs
- **cancel_ongoing_request**: Stop signature process
- **create_yousign_contact**: Add to address book
- **create_signature_request**: Start new signature process
- **delete_signature_request**: Remove draft request
- **get_audit_trail_link**: Get evidence file link
- **get_signature_request**: Get request status
- **get_workspace_details**: Get account info
- **list_yousign_contacts**: List address book
- **list_signature_requests**: List all requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yousign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new signature request named 'Annual Service Agreement'."

**🤖 AI Agent:**
> I've created the signature request 'Annual Service Agreement' (ID: req_8829). It's currently in draft status. Would you like to add signers or documents now?

---

**👤 You:**
> "Check the status of my ongoing signature requests."

**🤖 AI Agent:**
> You have 2 ongoing requests. 'Employment Contract' is pending signatures from 1 recipient, and 'NDA 2024' is fully signed and ready for download.


## Installation & Usage

To install and use the **Yousign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yousign-alternative](https://vinkius.com/mcp/yousign-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
