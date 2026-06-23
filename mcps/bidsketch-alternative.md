# Bidsketch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bidsketch-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Win more clients with beautiful proposals that track views, collect e-signatures, and accelerate your sales cycle.

## Description
Connect your **Bidsketch** account to any AI agent and take full control of your professional sales proposals and client management workflows through natural conversation.

### What you can do

- **Proposal Orchestration** — List and manage all sales proposals programmatically, retrieving detailed status, high-fidelity values, and associated client metadata in real-time
- **Client Relationship Management** — Programmatically create and manage your directory of prospects and organizations to maintain a perfectly coordinated sales database
- **Template Intelligence** — Access and monitor your library of proposal templates to ensure your high-fidelity brand styling and content are consistently applied
- **Deal Tracking Architecture** — Retrieve granular details for specific proposals, including pricing components and high-fidelity descriptions directly through your agent
- **Sales Visibility Monitoring** — Access comprehensive overviews of your active proposal pipeline and client growth to coordinate your revenue operations efficiently

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your Bidsketch account settings (Settings > API)
3. Start orchestrating your sales documents and clients from Claude, Cursor, or any MCP client

No more manual status checking or missing high-intent buyer views. Your AI acts as your dedicated sales operations coordinator and proposal architect.

### Who is this for?

- **Account Executives** — instantly retrieve proposal summaries and update client records using natural language commands
- **Freelancers & Agencies** — automate the creation of professional quotes and monitor prospect engagement without leaving your workspace
- **Sales Managers** — monitor the active proposal pipeline and coordinate client databases through simple AI queries


## Available Tools (6)
- **create_client**: Create a new client
- **create_proposal**: Pass data as a JSON string.

Create a new proposal
- **get_proposal_details**: Get specific proposal details
- **list_clients**: List all clients
- **list_proposals**: List all sales proposals
- **list_templates**: List all proposal templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bidsketch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active sales proposals in Bidsketch."

**🤖 AI Agent:**
> I've retrieved your proposals. You currently have 5 active documents, including 'Website Redesign' (Status: Sent) and 'SEO Strategy'. Would you like the high-fidelity pricing metadata for any of these?

---

**👤 You:**
> "Create a new client 'John Doe' (john@example.com) for 'Acme Corp'."

**🤖 AI Agent:**
> Client created! John Doe has been successfully added to your Bidsketch directory (ID: cli_789). He is now available for proposal association. Shall I list your available templates for him?

---

**👤 You:**
> "Show the status and value for proposal ID 'prop_123'."

**🤖 AI Agent:**
> Fetching proposal details... Proposal prop_123 ('Global Logistics Pilot') is currently 'Viewed' with a total value of $5,400.00. Shall I retrieve the high-fidelity fee breakdown for you?


## ❓ FAQ

**Q: How do I find my Bidsketch API Token?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique personal token.

**Q: Can I use specific templates via AI?**
Yes! Use the `list_templates` tool to identify the correct ID, and then specify it when creating a new proposal programmatically.

**Q: How do I track if a proposal was sent?**
Use the `list_proposals` or `get_proposal_details` tools to retrieve the current status (Draft, Sent, Viewed, Won) of any document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bidsketch-alternative](https://vinkius.com/mcp/bidsketch-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bidsketch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bidsketch-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bidsketch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bidsketch-alternative": {
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
