# Keepcon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keepcon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate content moderation and semantic analysis via Keepcon.

## Description
Empower your AI agents to moderate user-generated content using **Keepcon**. This MCP server enables seamless integration with Keepcon's semantic moderation engine for both real-time and batch processing.

### What you can do

- **Real-time Moderation** — Submit text for immediate moderation decisions (approve/reject) and category tagging
- **Batch Processing** — Import large volumes of content for asynchronous moderation and retrieve results in bulk
- **Result Management** — Export pending moderation decisions and acknowledge processed results to maintain a clean queue
- **Feedback Loop** — Submit feedback on moderation decisions to improve the accuracy of the semantic engine
- **Profile Insight** — List and query user profiles associated with moderated content

### How it works

1. Subscribe to this server
2. Enter your Keepcon API Key and Account Number
3. Start moderating content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — Automate the moderation of forums, chats, and social comments effortlessly
- **Security Teams** — Monitor and filter incoming content for policy compliance via natural language
- **Developers** — Integrate semantic moderation checks into your applications during development


## Available Tools (9)
- **acknowledge_results**: Acknowledge receipt of results
- **export_results**: Retrieve batch moderation results
- **submit_feedback**: g., false positives) to improve the semantic engine.

Submit moderation feedback
- **get_profile_by_social_id**: g., twitter, facebook) and the network-specific user ID.

Get a user profile by social network ID
- **get_profile**: Get a specific user profile by Keepcon ID
- **import_batch**: Returns an import ID.

Submit content for batch moderation
- **moderate_content**: Returns the decision (approve/reject) and tags.

Moderates content in real-time
- **list_profiles**: List user profiles
- **search_profiles**: Search profiles with filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keepcon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Moderate this text in the 'forum' context: 'This user is being very aggressive!'"

**🤖 AI Agent:**
> I've processed the text. Keepcon's decision is 'REJECT' with the tag 'Aggressive Behavior'. Would you like to see more details?

---

**👤 You:**
> "Export pending moderation results for the 'chat' context."

**🤖 AI Agent:**
> I've retrieved 15 pending results for context 'chat'. 12 were approved and 3 were rejected. The result set ID is 'SET_98765'.

---

**👤 You:**
> "List all user profiles in my Keepcon account."

**🤖 AI Agent:**
> I found 50 user profiles. Notable users include 'user_abc' (Twitter) and 'user_xyz' (Facebook).


## ❓ FAQ

**Q: What is the difference between synchronic and asynchronic moderation?**
Synchronic (`moderate_content`) provides an immediate decision, while asynchronic (`import_batch`) is for large volumes where results are retrieved later via the export tool.

**Q: How do I ensure results are not exported twice?**
After retrieving results with `export_results`, use the `acknowledge_results` tool with the corresponding `set_id` to confirm processing.

**Q: Can I provide feedback on incorrect moderation decisions?**
Yes, use the `submit_feedback` tool to report false positives or negatives, helping the Keepcon engine learn and improve over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keepcon](https://vinkius.com/mcp/keepcon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keepcon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keepcon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keepcon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keepcon": {
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
