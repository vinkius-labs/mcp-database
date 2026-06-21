# Chanty MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chanty)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate team communication via Chanty — manage conversations, send messages, invite members, and update statuses using any AI agent.

## Description
Connect your **Chanty** workspace to any AI agent and command your team's communication flow naturally. Bypass the UI and construct high-speed chat operations through simple prompts.

### What you can do

- **Messages** — Send targeted messages to any conversation, retrieve chat histories, and delete texts as needed
- **Conversations** — Create entirely new channels, list active ones, and irreversibly vaporize outdated spaces
- **Members** — Inspect company directories, track user IDs, and instantly dispatch email invitations to onboard new users
- **Profile & Status** — Verify token limits and globally mutate your web CRM status icon automatically

### How it works

1. Subscribe to this server
2. Enter your Chanty API Token
3. Start architecting discussions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project managers** — bootstrap new channels for incoming projects and invite the whole squad automatically
- **Developers & DevOps** — dump log outputs and notifications into designated Chanty channels straight from the agent
- **HR & Ops** — seamlessly onboard new members to the workspace and specific rooms with one command


## Available Tools (10)
- **create_conversation**: Bootstrap an entirely empty structural chat Room dynamically
- **delete_conversation**: Irreversibly vaporize explicit Channel spaces terminating histories
- **delete_message**: Obliterate mapped HTTP bounds removing specific Texts
- **list_messages**: Identify bounded routing spaces verifying explicit historical messages
- **get_profile**: Inspect deep internal arrays evaluating self-assigned permissions
- **invite_member**: Dispatch an automated JSON block emitting email triggers
- **list_conversations**: Perform structural extraction of properties driving active Chanty layouts
- **list_members**: Retrieve explicit Directory maps tracking User IDs
- **send_message**: Provision a highly-available JSON Payload dropping messages into Chanty Chats
- **set_status**: Mutate global Web CRM boundaries substituting plain Status texts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chanty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We just signed a new client. Create a 'project-titan' conversation and invite 'alex@domain.com'."

**🤖 AI Agent:**
> The public conversation 'project-titan' has been created successfully. The email trigger for 'alex@domain.com' was also dispatched natively! Should I drop a welcome message inside?

---

**👤 You:**
> "Please mark my profile status to 'In deep focus mode' for the rest of the day."

**🤖 AI Agent:**
> Done, status translated and globally substituted on your profile. Your team will now see 'In deep focus mode' effectively. I will keep it that way. Anything else I can do?

---

**👤 You:**
> "Can you delete the message I just sent in the 'general' channel? I made a typo."

**🤖 AI Agent:**
> I've pulled the recent chat logs for 'general', identified the UUID block mapping your latest text, and successfully executed the removal. The error is vaporized! Need me to send a corrected payload?


## ❓ FAQ

**Q: Can my AI agent set up project channels automatically?**
Yes. Ask the agent to create a new conversation and list members from your directory. It will bootstrap the empty room dynamically, allowing you to instantly share the link or invite employees to start discussing immediately.

**Q: How can I invite new hires into the Chanty workspace without opening the UI?**
Just provide your agent with a list of emails. It utilizes the `/invites` endpoint to dispatch automated onboarding emails, bypassing the manual web forms and integrating new users smoothly.

**Q: Can the agent clean up our workspace by deleting obsolete channels?**
Absolutely. It can list all active conversations to identify unused chat limits. Once confirmed, tell the agent to delete specific groups. It triggers an irreversible HTTP DELETE execution, keeping your team space cleanly organized.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chanty](https://vinkius.com/mcp/chanty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chanty** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chanty` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chanty** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chanty": {
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
