# FadaDa / 法大大 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fadada)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Leading digital signature and contract platform in China — manage sign flows, templates, and documents via AI.

## Description
Empower your AI agent to orchestrate your digital agreement lifecycle with **FadaDa** (法大大), the premier electronic signature platform in China. By connecting FadaDa to your agent, you transform complex contract workflows and document signing into a natural conversation. Your agent can instantly list your sign flows, create new signature tasks, manage document templates, and even retrieve signing URLs for participants without you ever needing to navigate the comprehensive FadaDa portal. Whether you are managing high-volume employee contracts or complex B2B agreements, your agent acts as a real-time legal operations assistant, keeping your documents secure and your business moving.

### What you can do

- **Sign Flow Orchestration** — Create and manage digital signature workflows with full support for documents and signers.
- **Template Management** — Browse predefined document templates to accelerate your contract production.
- **Signature Tracking** — Monitor the real-time status of active sign flows and retrieve execution URLs for participants.
- **Document Control** — Add PDF documents to signature tasks and retrieve download links for completed agreements.
- **Organization Insights** — Retrieve high-level information about your enterprise FadaDa account and authorization status.

### How it works

1. Subscribe to this server
2. Enter your FadaDa App ID and App Secret
3. Start managing your digital agreements through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Operations** — automate contract creation and monitor signing progress through natural language queries.
- **HR Managers** — manage employment contracts and internal policy acknowledgments directly from your AI-powered workspace.
- **Sales Operations** — coordinate B2B agreements and monitor client signatures via a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide document execution and compliance status.


## Available Tools (10)
- **add_fadada_docs**: Add documents to flow
- **add_fadada_signers**: Add signers to flow
- **create_fadada_sign_flow**: Create a new sign flow
- **download_fadada_docs**: Download flow documents
- **get_fadada_execute_url**: Get signature URL
- **get_fadada_org_info**: Get organization details
- **get_fadada_sign_flow**: Get sign flow details
- **list_fadada_sign_flows**: List sign flows
- **list_fadada_templates**: List sign templates
- **start_fadada_flow**: Start sign flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FadaDa / 法大大** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active signature flows on FadaDa."

**🤖 AI Agent:**
> I've retrieved your active FadaDa flows. You have 5 tasks in progress, including 'Service Agreement - Client A' and 'New Employee Offer'. Which one would you like to check the status for?

---

**👤 You:**
> "Get the signing URL for account 'acc-8821' in flow 'flow-9920'."

**🤖 AI Agent:**
> I've retrieved the execution URL for the participant. You can send this link to the signer to complete the process: [URL].

---

**👤 You:**
> "Show me all available document templates."

**🤖 AI Agent:**
> I've listed your FadaDa document templates. You have 3 templates ready for use: 'Standard NDA', 'Employment Contract v2', and 'Sales Agreement'. Would you like to use one of these for a new sign flow?


## ❓ FAQ

**Q: How do I find my FadaDa App ID and Secret?**
Log in to the [FadaDa Open Platform](https://open.fadada.com/), create a new application, and you will find your App ID and App Secret in the application credentials section.

**Q: Can I retrieve the signing URL for a participant?**
Yes. Use the `get_fadada_execute_url` tool with the flow ID and the signer's account ID. Your agent will retrieve the unique URL where the participant can perform the signature.

**Q: Is it possible to download the signed documents?**
Yes! Once a sign flow is completed, you can use the `download_fadada_docs` tool to retrieve temporary download links for all documents included in that flow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fadada](https://vinkius.com/mcp/fadada)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FadaDa / 法大大** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fadada` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FadaDa / 法大大** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fadada": {
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
