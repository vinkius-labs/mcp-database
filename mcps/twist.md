# Twist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration-tools](../categories/collaboration-tools.md)

Automate asynchronous communication workflows via Twist — manage workspaces, channels, threads, comments, and direct messages via any AI agent.

## Description
Connect your **Twist** account to any AI agent and take full control of your team’s asynchronous, distraction-free dialogue through natural conversation.

### What you can do

- **Workspaces & Members** — Identify top-level organizations actively driving your team and find all associated workspace user accounts
- **Channels & Groups** — List open organizational categories holding specific deep-threaded discussions within your sub-department
- **Thread Execution** — Spark a new asynchronous discussion into a channel by writing full markup elements and posting deep remarks over an existing subject
- **Direct Messaging** — Access any active 1-on-1 conversations and directly parse long direct messages, modify recent text errors, or append comments rapidly

### How it works

1. Subscribe to this server
2. Enter your Twist API Token via the Developer Portal
3. Leverage your new communications assistant connecting securely from Claude, Cursor, or any MCP-compatible environment

No more switching contexts and scrambling to find important threads on standard messaging software. Twist’s architecture works seamlessly inside an agentic command center to let you focus.

### Who is this for?

- **Product Managers** — spin up new announcement threads with structured markdown summaries to specific channels
- **Engineering Teams** — auto-read debugging or release threads asynchronously skipping massive chat floods
- **Remote employees** — query your PM's 1-on-1 direct messages to catch up without an actual video-call


## Available Tools
- **create_comment**: Provide the thread_id and your message.

Posts a reply to an existing thread
- **send_direct_message**: Provide conversation_id and content.

Sends a private message to a specific conversation
- **create_thread**: Provide channel_id, title, and initial content.

Creates a new asynchronous discussion thread in a channel
- **list_channels**: Provide the workspace_id.

Lists all channels within a specific Twist workspace
- **list_direct_messages**: Provide the conversation_id.

Lists messages from a specific 1-on-1 direct conversation
- **list_threads**: Provide the channel_id.

Lists all conversation threads within a specific channel
- **list_workspace_users**: Lists all members of a specific workspace
- **list_workspaces**: Identify bounded Twist Workspaces actively driving Async Teams
- **update_direct_message**: Provide the message_id.

Modifies a previously sent direct message
- **update_thread**: Provide the thread_id.

Updates the title or content of an existing thread


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize all responses in the 'Q3 Pipeline' thread to see where we landed."

**🤖 AI Agent:**
> I've pulled 12 responses from the 'Q3 Pipeline' thread. The team decided to focus on Enterprise features and push the Analytics sprint to Q4. Sara mentioned the scoping doc is finalized. Should I prepare a comment indicating your alignment?

---

**👤 You:**
> "Post a new thread to the #bugs channel describing the latency issue in the EU region."

**🤖 AI Agent:**
> I've created a new thread titled '[SEV-2] Extremely high latency on EU DB shards'. The content is fully formatted, including your ping logs and initial analysis. Thread ID is 44351.

---

**👤 You:**
> "Check all my PMs with Mark and see if he shared his Figma files yesterday."

**🤖 AI Agent:**
> I've reviewed your direct messages with Mark. Yesterday afternoon, he mentioned sharing a link via Figma, and left the exact URL 'figma.com/design/xyz'. No physical attachments dot-zip were detected.


## ❓ FAQ

**Q: Can my AI automatically create a new thread with bug report details in the #dev channel?**
Yes. Once you invoke the agent to query the channel ID for '#dev', it can execute the thread creation workflow and post an entire Markdown-formatted issue payload perfectly directly to the interface.

**Q: Is it possible to correct a message typo via the agent?**
Yes! Twist is unique in allowing asynchronous editing. By providing your exact Message ID, the AI agent can overwrite and patch up your old text block retaining timeline flow naturally.

**Q: Can the agent fetch recent threaded responses to summarize an ongoing project decision?**
Absolutely. It pulls in heavy threads natively. Give the agent a thread ID and request a summarization—it will digest long chains of conversation and outline the top project consensus within seconds avoiding you long reading phases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twist](https://vinkius.com/mcp/twist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `twist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twist": {
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
