# Concord CLM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/concord-clm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Enable your AI agent to manage contracts, send documents for signature, and track agreement statuses via the Concord CLM API.

## Description
Connect your AI assistant to **Concord**, the Contract Lifecycle Management (CLM) platform that centralizes how your team drafts, negotiates, signs, and stores contracts.

### What you can do

- **Agreement Lookup** — Search and retrieve any contract by name, ID or status directly through your AI chat.
- **Signature Workflows** — Send agreements out for e-signature to internal or external parties without leaving your conversation.
- **Template-Based Creation** — Create new agreements from pre-approved templates, automatically populating fields and routing them for review.

### How it works

1. Add the Concord CLM integration to your AI toolset.
2. Enter your API Key (found under Global Settings > API Keys in the Concord dashboard).
3. Start managing your contracts via natural language commands.

### Who is this for?

- **Legal Teams** — Quickly locate specific agreement clauses or check signature statuses without navigating the full Concord UI.
- **Procurement Managers** — Speed up vendor onboarding by creating and routing contracts directly from chat.
- **Operations Leaders** — Get instant visibility into contract pipeline and approval bottlenecks.


## Available Tools
- **create_agreement**: Create a new agreement in Concord
- **get_agreement**: Retrieve detailed information about a specific agreement
- **get_current_user**: Retrieve details of the currently authenticated user
- **list_signed_agreements**: Quickly list all fully signed agreements
- **list_agreements**: Retrieve a list of agreements from Concord CLM
- **list_templates**: Retrieve a list of document templates available in Concord
- **list_users**: Retrieve a list of all users in your Concord organization
- **list_webhooks**: Retrieve a list of configured webhooks
- **search_agreements_by_name**: Find agreements by their name
- **send_for_signature**: Trigger the signature process for a specific agreement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concord CLM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all signed contracts in Concord."

**🤖 AI Agent:**
> I found 12 signed agreements in your Concord account. Here are the most recent:
1. 'Vendor Agreement — Acme Corp' (signed Jan 15)
2. 'NDA — Beta Partners' (signed Jan 10)
3. 'Service Contract — Delta Inc' (signed Dec 28)
Would you like details on any of these?

---

**👤 You:**
> "Send agreement 'agr-4521' for signature."

**🤖 AI Agent:**
> Done! Agreement 'agr-4521' has been sent for signature to all designated parties. You'll receive a notification once all signatures are collected.

---

**👤 You:**
> "Check the status of agreement ID 'agr-8901'."

**🤖 AI Agent:**
> Agreement 'agr-8901' (Marketing Retainer) is currently in the 'Review' stage. It is pending approval from Sarah Jenkins.


## ❓ FAQ

**Q: How do I get my Concord API key?**
Log in to the Concord web app, go to **Global Settings > API Keys**, and generate a new key. Copy it and paste it into the authentication field below.

**Q: Does this work with the Sandbox environment?**
Yes. Set 'Use Sandbox?' to true in the credentials configuration to connect to the UAT environment instead of production.

**Q: Can I create documents from templates?**
Yes. When using the 'create_agreement' tool, you can specify a templateId to generate a document based on a pre-existing template.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/concord-clm](https://vinkius.com/mcp/concord-clm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concord CLM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `concord-clm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concord CLM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concord-clm": {
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
