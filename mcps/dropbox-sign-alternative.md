# Dropbox Sign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox-sign-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dropbox-sign-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dropbox-sign-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Get documents signed electronically with legally binding e-signatures, templates, and audit trails your business can trust.

## Description
Connect your **Dropbox Sign** (formerly HelloSign) account to any AI agent and take full control of your electronic signature and document automation workflows through natural conversation.

### What you can do

- **Request Orchestration** — List and manage signature requests programmatically, including monitoring signer status and document completion in real-time
- **Automated Sending** — Programmatically create new signature requests using file URLs or predefined templates to streamline your legal operations
- **Template Intelligence** — Access your directory of document templates and retrieve detailed metadata about roles and fields to maintain high-fidelity automation
- **Asset Retrieval** — Programmatically generate secure download links or retrieve Base64 Data URIs for finalized signed PDF documents
- **Operational Visibility** — Monitor bulk sending jobs, manage unclaimed drafts, and check account usage limits directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Dropbox Sign dashboard (Settings > API)
3. Start managing your e-signature pipeline from Claude, Cursor, or any MCP client

No more manual status checking or digging through contract folders. Your AI acts as your dedicated legal and document operations coordinator.

### Who is this for?

- **Legal & Compliance Teams** — instantly track the status of critical agreements and retrieve signed copies using natural language
- **HR Operations** — automate the dispatch of onboarding documents and monitor signer progress without leaving your workspace
- **Sales Teams** — create and send contract templates directly through simple AI queries to close deals faster


## Available Tools
- **cancel_signature_request**: Cancel a pending signature request
- **create_unclaimed_draft**: Create an unclaimed draft
- **get_account_info**: Get Dropbox Sign account details
- **get_files_data_uri**: Get document as Data URI
- **get_files_download_url**: Get temporary download link for files
- **get_signature_request_details**: Get details for a signature request
- **get_template_details**: Get template metadata
- **list_bulk_send_jobs**: List bulk sending jobs
- **list_signature_requests**: List all signature requests
- **list_templates**: List available signature templates
- **send_signature_request**: Send a document for signature
- **send_with_template**: Send signature request using templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dropbox Sign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my pending signature requests and their status."

**🤖 AI Agent:**
> I've retrieved your active requests. You have 3 documents awaiting signature, including 'NDA - Project Alpha' and 'Sales Agreement #402'. Would you like the signer details for any of these?

---

**👤 You:**
> "Send the 'Agreement' template to 'john.doe@example.com'."

**🤖 AI Agent:**
> Signature request dispatched! I've successfully sent the 'Agreement' template to John Doe. The request ID is 'req_123'. I'll alert you as soon as they view or sign the document.

---

**👤 You:**
> "Get the download link for the signed document 'req_123'."

**🤖 AI Agent:**
> Link generated! You can download the finalized PDF for request req_123 here: [download_url]. The link is secure and will expire in 24 hours.


## Installation & Usage

To install and use the **Dropbox Sign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox-sign-alternative](https://vinkius.com/mcp/dropbox-sign-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
