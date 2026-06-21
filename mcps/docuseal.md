# DocuSeal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docuseal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docuseal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docuseal-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document signing workflows via DocuSeal — manage templates, send signature requests, and track signers directly from any AI agent.

## Description
Connect your **DocuSeal** account to any AI agent to streamline your electronic signature processes through natural language. This MCP server provides full control over document templates and signing lifecycles.

### What you can do

- **Template Management** — List, create, and update document templates. You can even generate new templates directly from HTML content.
- **Signature Requests** — Create new submissions (signature requests) by linking templates to specific signers and choosing whether to send automated emails.
- **Signer Tracking** — Retrieve detailed information about submitters and monitor the progress of individual signature requests.
- **Data Pre-filling** — Update submitter information or pre-fill form fields programmatically before the document is sent for signing.
- **Document Archiving** — Manage the lifecycle of your documents by retrieving or deleting templates and submissions as needed.

### How it works

1. Subscribe to this server
2. Enter your DocuSeal API Key
3. Start managing contracts and signatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations & HR** — Automate the generation of employment contracts and onboarding documents.
- **Legal Teams** — Quickly query the status of pending agreements and manage standard legal templates.
- **Sales Teams** — Send out sales orders and service agreements for signature without leaving your AI-powered workflow.


## Available Tools
- **create_submission**: Create a new submission to request signatures
- **create_template**: Can be created from HTML content.

Create a new template from HTML
- **delete_submission**: Cancel or delete a submission
- **delete_template**: Archive or delete a template
- **get_submission_documents**: Get download URLs for signed documents
- **get_submission**: Retrieve details of a specific submission
- **get_submitter**: Retrieve details about a specific signer
- **get_template**: Retrieve a specific template by ID
- **list_submissions**: List all submissions
- **list_templates**: List all document templates
- **update_submitter**: Update signer information or pre-fill fields
- **update_template**: Update an existing template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocuSeal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available document templates in DocuSeal."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 active templates: 'NDA 2024' (ID: 101), 'Service Agreement' (ID: 102), and 'Onboarding Form' (ID: 103).

---

**👤 You:**
> "Create a signature request for template 102 for john@example.com."

**🤖 AI Agent:**
> Submission created successfully. A signature request for the 'Service Agreement' has been sent to John (john@example.com). Submission ID: 5001.

---

**👤 You:**
> "Check the status of the signer with ID 88291."

**🤖 AI Agent:**
> Signer 'Alice Smith' (ID: 88291) has received the document but has not signed it yet. The last update was 2 hours ago.


## Installation & Usage

To install and use the **DocuSeal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docuseal](https://vinkius.com/mcp/docuseal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
