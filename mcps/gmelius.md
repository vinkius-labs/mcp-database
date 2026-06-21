# Gmelius MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gmelius)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn Gmail into a collaborative workspace with shared inboxes, email delegation, and workflow automation for teams.

## Description
Connect your **Gmelius** account to any AI agent and take full control of your team's collaborative workspace and high-fidelity shared inbox orchestration through natural conversation.

### What you can do

- **Conversation Portfolio Orchestration** — List all collaborative email threads, retrieve detailed high-fidelity history, and monitor ticket status programmatically
- **Kanban Pipeline Intelligence** — Query team project boards, retrieve detailed technical metadata, and stay on top of workflow progress in real-time
- **Card & Task Orchestration** — Programmatically generate new task cards or email items on specific boards directly through your agent for perfectly coordinated delivery
- **Sequence Monitoring** — Access configured automated high-fidelity email sequences and monitor their status directly through your agent for outreach optimization
- **Template Discovery** — Access your complete directory of high-fidelity shared email templates and inboxes to choose the right context for every interaction
- **Operational Monitoring** — Verify account-level API connectivity and monitor collaborative volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from your Gmelius dashboard (Settings > API)
3. Start managing your collaborative growth from Claude, Cursor, or any MCP client

No more manual status updates or jumping between shared inboxes. Your AI acts as your dedicated collaboration coordinator and shared inbox architect.

### Who is this for?

- **Team Leads** — instantly retrieve project board statuses and monitor team responsiveness using natural language commands without leaving your creative workspace
- **Customer Success Managers** — verify high-fidelity conversation history and manage shared tags to ensure healthy client relationships
- **Operations Managers** — analyze collaborative workflows and monitor sequence performance through simple AI queries


## Available Tools
- **create_gmelius_card**: Add a new card to a board
- **get_gmelius_board**: Get details for a specific board
- **get_gmelius_conversation**: Get details for a specific conversation
- **list_gmelius_boards**: List collaborative Kanban boards
- **list_gmelius_board_cards**: List cards on a Kanban board
- **list_gmelius_conversations**: List Gmelius shared conversations
- **list_gmelius_sequences**: List email sequences
- **list_gmelius_templates**: List shared email templates
- **check_gmelius_status**: Check API Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gmelius** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Kanban boards and show their status."

**🤖 AI Agent:**
> I've retrieved your boards. You currently have 3 active high-fidelity boards, including 'Sales Pipeline' and 'IT Support'. Would you like the detailed health metadata for any of them?

---

**👤 You:**
> "Show the last 5 conversations assigned to me."

**🤖 AI Agent:**
> Inbox orchestrated! I've identified 5 recent high-fidelity conversations. I've retrieved the technical status and last message for your review. Shall I summarize the progress?

---

**👤 You:**
> "Check the available email templates for the 'Sales' team."

**🤖 AI Agent:**
> Template directory orchestrated! Your team currently has 10 high-fidelity profiles available for interactions. Your API connection is healthy. Shall I retrieve the detailed metadata for the most used template?


## ❓ FAQ

**Q: How do I find my Gmelius Access Token?**
Log in to your account, navigate to **Account Settings** > **API**, and register a new high-fidelity **API App** to obtain your Bearer token.

**Q: Can I check board card details via AI?**
Yes! The `list_gmelius_board_cards` tool allows your agent to retrieve high-fidelity metadata including description and status for all cards on a board.

**Q: How do I list my shared email sequences?**
Use the `list_gmelius_sequences` tool to retrieve the complete high-fidelity directory of automated sequences along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gmelius](https://vinkius.com/mcp/gmelius)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gmelius** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gmelius` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gmelius** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gmelius": {
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
