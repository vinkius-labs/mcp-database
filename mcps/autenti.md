# Autenti MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autenti)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Sign documents digitally with legal-grade electronic signatures that comply with European eIDAS regulations.

## Description
Connect your **Autenti** account to any AI agent and take full control of your professional document signing workflows and e-signature compliance through natural conversation.

### What you can do

- **Process Orchestration** — List and manage document signature processes programmatically, retrieving detailed status, high-fidelity metadata, and historical audit data in real-time
- **Dynamic Lifecycle Management** — Discover and execute available actions (Send, Sign, Reject) based on the document's current state to coordinate complex signature workflows
- **Participant Intelligence** — Programmatically add signers and observers to your processes and manage your organizational contact directory to ensure perfectly coordinated collaboration
- **Event Monitoring** — Access and monitor your complete directory of webhooks to receive real-time notifications for incoming document events directly through your agent
- **Operational Visibility** — Access high-fidelity profile metadata for your authenticated user and verify API connectivity directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **OAuth Access Token** from the Autenti Developer Portal
3. Start managing your digital trust pipeline from Claude, Cursor, or any MCP client

No more manual status checking of individual contracts or digging through fragmented email threads. Your AI acts as your dedicated digital signature coordinator and compliance architect.

### Who is this for?

- **Legal & Compliance Teams** — instantly retrieve process statuses and execute signature actions using natural language commands
- **Sales Professionals** — automate the dispatch of agreements and monitor signer progress without leaving your creative workspace
- **HR Managers** — orchestrate employment contract workflows and manage participant directories through simple AI queries


## Available Tools
- **check_api_health**: Verify Autenti API connectivity
- **add_new_contact**: Add a contact to your address book
- **create_new_signature_process**: Requires a title and metadata.

Start a new document process
- **execute_process_action**: Use list_available_process_actions first to find valid names.

Execute a discovered action (e.g., Send, Sign, Reject)
- **get_user_account_profile**: Get authenticated user profile
- **get_process_details**: Get details for a specific signature process
- **list_available_process_actions**: Discover possible actions for a process
- **list_saved_contacts**: List your address book contacts
- **list_process_files**: List files within a process
- **list_process_participants**: List signers and observers
- **list_signature_processes**: List all document signature processes
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Autenti** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active document signature processes."

**🤖 AI Agent:**
> I've retrieved your active processes. You currently have 3 documents in progress, including 'Service Agreement' (Status: SENT) and 'NDA'. Would you like the detailed participant metadata for any of these?

---

**👤 You:**
> "What actions can I take on process 'proc_123'?"

**🤖 AI Agent:**
> For process proc_123, you can currently perform the following high-fidelity actions: 'SIGN_DOCUMENT', 'REJECT', or 'CANCEL'. Shall I proceed with the signature for you?

---

**👤 You:**
> "Add 'John Doe' (john@example.com) to my Autenti contacts."

**🤖 AI Agent:**
> Contact created! John Doe has been successfully added to your Autenti address book (ID: cont_456). He is now available for process association. Shall I start a new signature workflow for him?


## ❓ FAQ

**Q: How do I find my Autenti Access Token?**
Log in to the [**Autenti Developer Portal**](https://developers.autenti.com/), navigate to your application settings, and generate an OAuth 2.0 Access Token.

**Q: Can I discover valid actions via AI?**
Yes! The `list_available_process_actions` tool retrieves a dynamic list of valid operations (like SEND or SIGN) based on the document's high-fidelity status.

**Q: How do I add a new contact programmatically?**
Use the `add_new_contact` tool to register a name and email in your Autenti address book for future high-fidelity signature requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autenti](https://vinkius.com/mcp/autenti)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Autenti** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `autenti` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Autenti** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autenti": {
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
