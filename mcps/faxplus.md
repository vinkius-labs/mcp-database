# Fax.Plus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faxplus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send and receive faxes digitally through a modern API without physical machines, keeping your business compliant and paperless.

## Description
Connect your **Fax.Plus** account to any AI agent and take full control of your digital telephony and fax workflows through natural conversation.

### What you can do

- **Fax Orchestration** — List and monitor all incoming and outgoing faxes and retrieve detailed status updates and delivery metadata programmatically
- **Automated Sending** — Programmatically send new faxes to any international number in E.164 format and add transmission comments directly through your agent
- **Telephony Management** — Search for and list available fax numbers across various countries and area codes to expand your business presence
- **Outbox Oversight** — Track active fax jobs and programmatically cancel pending transmissions before they are completed to save resources
- **Account Visibility** — Retrieve complete profile information, assigned numbers, and team member directories to maintain high-fidelity oversight

### How it works

1. Subscribe to this server
2. Retrieve your **Personal Access Token** from Fax.Plus (Settings > Integrations)
3. Start managing your digital faxing from Claude, Cursor, or any MCP client

No more manual status checking or complex form navigation in the fax dashboard. Your AI acts as your dedicated digital fax and telephony coordinator.

### Who is this for?

- **Operations Managers** — instantly check fax delivery statuses and manage telephony infrastructure using natural language commands
- **Legal & Admin Teams** — automate the sending of critical documents and track receipt without leaving your workspace
- **Business Development** — quickly find and assign new international fax numbers through simple AI queries


## Available Tools (8)
- **get_fax_details**: Includes information about the recipient, sender, and delivery status.

Get details for a specific fax
- **list_faxes**: Use this to monitor communication history and obtain fax IDs.

List received and sent faxes
- **list_fax_numbers**: Includes the number itself and its activation status.

List all assigned fax numbers
- **list_outbox_jobs**: Useful for monitoring ongoing transmissions.

List active or pending fax jobs
- **search_available_numbers**: Useful for expanding telephony infrastructure.

Search for available fax numbers
- **send_fax**: Requires the recipient phone number in E.164 format and allows for optional comments. Files are typically managed via the Fax.Plus outbox logic.

Send a new digital fax
- **get_account_info**: Use this to determine the current identity and account context.

Retrieve current Fax.Plus account details
- **cancel_outbox_job**: Requires the unique outbox job ID.

Cancel a pending fax job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fax.Plus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 received faxes."

**🤖 AI Agent:**
> I've retrieved your recent faxes. You have 5 received documents, including one from '+1234567890' arrived this morning. Would you like the detailed status or ID for any of them?

---

**👤 You:**
> "Send a fax to +15551234567 with comment 'Urgent review required'."

**🤖 AI Agent:**
> Fax triggered! I've initiated the transmission to +15551234567. The outbox job ID is 'job_123'. I'll monitor the delivery status and let you know when it's completed.

---

**👤 You:**
> "Search for available fax numbers in United Kingdom (country code: gb)."

**🤖 AI Agent:**
> Searching numbers... I've found 5 available fax numbers in the UK. Notable options include London (+44 20) and Manchester area codes. Would you like the full list of numbers and their activation status?


## ❓ FAQ

**Q: How do I find my Personal Access Token?**
Log in to your Fax.Plus dashboard, navigate to **Settings** > **Integrations**, and generate a new token under the Personal Access Token section.

**Q: What is the correct format for fax numbers?**
Fax numbers must be in international E.164 format, including the plus sign and country code (e.g., +1234567890).

**Q: Can I cancel a fax before it is sent?**
Yes! Use the `cancel_outbox_job` tool with the unique outbox job ID to stop a transmission that is still pending or sending.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faxplus](https://vinkius.com/mcp/faxplus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fax.Plus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `faxplus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fax.Plus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "faxplus": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
