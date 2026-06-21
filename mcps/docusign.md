# DocuSign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docusign)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docusign-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docusign-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send documents for signature, manage envelopes, track signing status, and automate contract workflows with AI.

## Description
Connect **DocuSign** to any AI agent and automate your entire contract lifecycle.

### What you can do

- **Envelope Management** — List, view, search, and send envelopes for signature
- **Template Library** — Browse and use pre-built templates for recurring documents
- **Recipient Tracking** — Check who has signed and who hasn't
- **Signing URLs** — Generate embedded signing links for instant signing
- **Void Envelopes** — Cancel pending signature requests
- **Folder Organization** — Browse envelope folders


## Available Tools
- **list_envelopes**: Provide a from_date in ISO format.

List envelopes (documents sent for signature)
- **search_envelopes**: Search envelopes by text
- **get_envelope**: Get envelope details
- **send_envelope**: Provide envelope definition as JSON.

Create and send a new envelope for signature
- **list_recipients**: List recipients of an envelope
- **list_templates**: List available envelope templates
- **get_template**: Get template details
- **void_envelope**: Requires a reason. This action is irreversible.

Void a sent envelope
- **list_folders**: List envelope folders
- **get_signing_url**: Provide envelope ID and recipient details as JSON.

Generate a signing URL for a recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocuSign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all envelopes from the last 30 days."

**🤖 AI Agent:**
> Found 8 envelopes:

1. **NDA - Acme Corp** — ✅ Completed
2. **Service Agreement** — ⏳ Awaiting signature
3. **Employment Contract** — ✅ Completed
...

---

**👤 You:**
> "Generate a signing link for the pending contract."

**🤖 AI Agent:**
> 🔗 Signing URL generated:

https://docusign.net/signing/xxxx

This link expires in 5 minutes.

---

**👤 You:**
> "List all available templates."

**🤖 AI Agent:**
> 5 templates available:

1. **Standard NDA** — 2 recipients
2. **Service Agreement** — 3 recipients
3. **Employment Offer** — 1 recipient
...


## Installation & Usage

To install and use the **DocuSign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docusign](https://vinkius.com/mcp/docusign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
