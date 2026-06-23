# Telegram Bot API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telegram-bot-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Connect your AI natively to Telegram. Read user messages, administrate chats, send push notifications, and automate media distribution directly from the prompt.

## Description
Transform your local conversational window into a powerful global messaging director natively integrating the **Telegram Bot** MCP module. By authorizing your LLM to act as a certified Telegram Bot application, you bypass standard messaging clients entirely. Pull pending texts, analyze incoming commands, send formatted automated replies, push file alerts, and survey complex group metrics strictly evaluating server parameters without any external GUI overhead.

### What you can do

- **Bi-Directional Messaging** — Dispatch alerts generating explicit payloads invoking `send_text_message` and instantly retrieve the latest interactions testing logic sequences via `list_bot_updates`.
- **Content Curation & Adjustments** — Modify previously broadcasted texts dynamically evaluating `edit_message_text` or permanently erase inappropriate replies extracting logs into `delete_chat_message`.
- **Media Syndication** — Broadcast digital assets seamlessly pushing web URLs natively into chats via `send_photo_by_url` and distributing structured documents executing `send_document_by_url`.
- **Group & Channel Auditing** — Interrogate logical permissions observing member status evaluating `list_chat_administrators` and confirm audience penetration executing `get_chat_member_count`.

### How it works

1. Provision the generic Telegram connectivity structure correctly inside your Vinkius limits module.
2. In Telegram, access `@BotFather`, request a new bot token natively, and assign the matrix code tightly as `TELEGRAM_BOT_TOKEN` within your local MCP authorization files.
3. Instruct your artificial assistant logically: "Check for any new messages sent to the bot inbox, find the user mentioning 'help', and reply to their chat_id with our documentation link."

### Who is this for?

- **Chatbots Prototype Developers** — Directly interrogate incoming JSON queries simulating conversations (`list_bot_updates`) explicitly without writing explicit backend parsing routes temporarily.
- **Community Managers** — Swiftly analyze organizational charts querying active managers via `list_chat_administrators` logging strict compliance textually navigating prompt outputs.
- **DevOps Engineers** — Construct rapid push-notification alerts pushing build failure pictures (`send_photo_by_url`) straight to dedicated on-call Telegram groups effortlessly.


## Available Tools (14)
- **delete_chat_message**: Bots can delete their own messages or those of users in groups they manage.

Permanently deletes a message from a chat
- **forward_message**: The original sender information is preserved.

Forward a message from one chat to another
- **get_chat_member**: Get information about a specific member in a chat
- **pin_chat_message**: Bot must have pin_messages permission.

Pin a message in a chat
- **unpin_chat_message**: Unpin a message from a chat
- **get_chat_details**: Retrieves detailed information about a chat (user, group, or channel)
- **get_bot_info**: Retrieves basic information about the bot (ID, username, etc.)
- **edit_message_text**: Requires the chat_id and the original message_id.

Edits the text of a previously sent message
- **list_chat_administrators**: Lists the administrators of a specific group or channel
- **get_chat_member_count**: Retrieves the total number of members in a specific chat
- **list_bot_updates**: You can provide an offset_id to skip older records.

Retrieves new messages and updates from users (Long Polling)
- **send_document_by_url**: Provide a chat_id and the direct download link.

Sends a file or document to a chat using a public URL
- **send_text_message**: Requires a valid chat_id.

Sends a text message to a specific chat or user
- **send_photo_by_url**: Provide a chat_id and an absolute HTTPS URL to the image.

Sends an image to a chat using a public URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telegram Bot API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan the bot updates, check for new interactions, and send a structured text message back to the latest user chat ID resolving their query."

**🤖 AI Agent:**
> Interrogating 'list_bot_updates' securely natively...
Found 2 recent updates. Extracting newest payload context. Chat ID: 8472910.
User asks: 'Server Status'.
Dispatching resolution dynamically utilizing 'send_text_message'. Payload correctly executed and transmitted to the Telegram Chat.

---

**👤 You:**
> "Send a markdown formatted message to the #engineering channel."

**🤖 AI Agent:**
> Formatting payload with `send_message`...
Message "Deployment to production has started. **Status: Green**" sent successfully to `@engineering_alerts` (ID: -100123456).

---

**👤 You:**
> "Fetch the last 5 messages from our customer support group."

**🤖 AI Agent:**
> Calling Telegram API (`get_updates`)...
Retrieved 5 recent messages from Chat ID -100987654:
1. User44: 'Is the API down?'
2. AgentSmith: 'No, looking into it...'
3. User44: 'My token is failing.'
4. AgentSmith: 'Can you DM me your client ID?'
5. User12: 'I have the same issue.'


## ❓ FAQ

**Q: Can it read incoming messages?**
Yes. Use `list_bot_updates` to pull the latest unacknowledged messages sent to your bot. This uses long polling — no webhook server required.

**Q: Can it send images and documents?**
Yes. Use `send_photo_by_url` and `send_document_by_url` to share media by providing a public URL. The files are delivered directly to the target chat.

**Q: How do I create a bot token?**
Open Telegram and message `@BotFather`. Send `/newbot`, follow the prompts to name your bot, and copy the HTTP API token it provides. Paste it into the field below.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telegram-bot-api](https://vinkius.com/mcp/telegram-bot-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telegram Bot API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `telegram-bot-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telegram Bot API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telegram-bot-api": {
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
