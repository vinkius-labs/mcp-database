# iFax MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ifax)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ifax-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ifax-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send and receive faxes from your phone or computer with cloud-based faxing that eliminates the need for physical machines.

## Description
Connect your **iFax** account to any AI agent and manage fax communications through natural conversation.

### What you can do

- **Send Faxes** — Transmit documents to fax numbers worldwide with delivery confirmation
- **Track Status** — Monitor real-time delivery status of sent faxes
- **Fax History** — Browse all sent and received faxes with timestamps and status
- **Cancel Pending** — Cancel faxes that haven't been transmitted yet
- **Resend Failed** — Retry failed fax transmissions automatically
- **Download Documents** — Retrieve received fax documents as files

### How it works

1. Subscribe to this server
2. Enter your iFax API Key
3. Start managing faxes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare** — send HIPAA-compliant faxes for medical records and prescriptions
- **Legal Teams** — transmit contracts, filings, and signed documents
- **Operations** — automate fax workflows for compliance and document exchange


## Available Tools
- **cancel_fax**: Cancel a pending fax
- **download_fax**: Download a fax document
- **get_fax_status**: Check fax delivery status
- **list_faxes**: List sent faxes
- **resend_fax**: Resend a failed fax
- **send_fax**: Pass faxData as a JSON string containing the file metadata and base64 content.

Send a new fax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iFax** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a fax with the Q2 report to +1-555-0123 and check its delivery status."

**🤖 AI Agent:**
> Fax sent! ID: fax_8921. Destination: +1-555-0123. Document: Q2_Report.pdf (4 pages). Status: Transmitting... ⏳. Updated: Status changed to ✅ Delivered. Transmission time: 45 seconds. Pages transmitted: 4/4. Confirmation: fax_8921_conf.pdf. Would you like to send another fax or view history?

---

**👤 You:**
> "Show my fax history and resend any that failed."

**🤖 AI Agent:**
> Fax history: 24 total. Delivered: 20, Failed: 3, Pending: 1. Failed faxes: 1) fax_8915 (+1-555-0456, busy signal). 2) fax_8918 (+44-20-7123, no answer). 3) fax_8919 (+49-30-1234, line error). Resending all 3... fax_8915 → ✅ Delivered on retry. fax_8918 → ⏳ Transmitting. fax_8919 → ✅ Delivered on retry. 2 of 3 resolved. Would you like to download received faxes?

---

**👤 You:**
> "Download the latest received fax and cancel the pending transmission."

**🤖 AI Agent:**
> Latest received fax: fax_recv_445. From: +1-555-0789 (Acme Legal Dept). Received: Apr 26, 10:15 AM. Pages: 3. Document downloaded: Contract_Amendment_v2.pdf (245 KB). Pending fax cancelled: fax_8920 (to +33-1-4567, Q1 Summary). Status: ❌ Cancelled. Refund: credited. Would you like to send a new fax or view the downloaded document?


## Installation & Usage

To install and use the **iFax** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ifax](https://vinkius.com/mcp/ifax)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
