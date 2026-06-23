# Convai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Build and manage conversational AI characters with backstory, narrative design, and knowledge banks for games and apps.

## Description
Connect your **Convai** account to any AI agent to orchestrate lifelike conversational characters. This MCP server provides full access to the Convai Engine, allowing you to design complex NPCs and digital beings through natural language.

### What you can do

- **Character Management** — Create, update, and delete characters with specific voices, backstories, and language support.
- **Narrative Design** — Toggle narrative-driven modes and manage sections and triggers to create branching storylines.
- **Knowledge Integration** — Upload and manage documents in the Knowledge Bank to give your characters deep domain expertise.
- **Conversation Analytics** — List chat sessions, retrieve session details, and evaluate conversation quality.
- **Real-time Interaction** — Generate starter conversations or connect live to test character responses and voices.

### How it works

1. Subscribe to this server
2. Enter your Convai API Key
3. Start building interactive characters from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — Create and iterate on NPC personalities and backstories directly from your workspace.
- **Narrative Designers** — Map out complex story triggers and narrative sections without leaving your AI assistant.
- **AI Researchers** — Evaluate conversation quality and manage knowledge banks for specialized conversational agents.


## Available Tools (25)
- **list_chat_sessions**: List chat sessions for a character
- **list_knowledge_bank**: List Knowledge Bank status
- **list_languages**: Returns supported languages
- **list_narrative_sections**: List narrative sections
- **list_narrative_triggers**: List narrative triggers
- **list_voices**: Returns available voices categorized by provider
- **toggle_narrative**: Toggle narrative driven mode for a character
- **connect_live**: Connect to Live API via WebRTC
- **create_character**: Create a new Convai character
- **create_narrative_section**: Create a narrative section
- **create_narrative_trigger**: Create a narrative trigger
- **delete_character**: Delete a Convai character
- **delete_knowledge_bank**: Delete a Knowledge Bank file
- **edit_narrative_section**: Edit a narrative section
- **evaluate_conversation**: Evaluate a conversation transcript based on custom attributes
- **generate_backstory**: Generate a character description
- **generate_starter_conversation**: Generate follow-up options
- **get_character**: Get details for a specific Convai character
- **get_chat_session_details**: Get details of a specific chat session
- **get_prompt**: Fetch prompt data for debugging or advanced configuration
- **get_response**: Get a response from a character
- **list_characters**: Returns all characters associated with the account
- **update_character**: Update an existing Convai character
- **update_knowledge_bank**: Update a Knowledge Bank file
- **upload_knowledge_bank**: Upload a file to the Knowledge Bank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Convai characters."

**🤖 AI Agent:**
> I've retrieved your characters. You have 3 active characters: 'Cyber Guard' (ID: char_123), 'Merchant Elara' (ID: char_456), and 'System AI' (ID: char_789).

---

**👤 You:**
> "Generate a backstory for a futuristic detective named Jax."

**🤖 AI Agent:**
> Using `generate_backstory`... Jax is a former Neo-Tokyo enforcer turned private eye after a high-stakes betrayal. He specializes in tracking rogue synthetics in the neon-lit underbelly of the city.

---

**👤 You:**
> "Show me the details for character ID char_123."

**🤖 AI Agent:**
> Fetching details for 'Cyber Guard' (char_123)... Voice: 'M-US-1', Backstory: 'A sentinel programmed to protect the vault...', Model: 'gpt-4o', Temperature: 0.7.


## ❓ FAQ

**Q: How do I create a new character with a specific voice?**
Use the `create_character` tool. You can specify the `charName`, `backstory`, and `voiceType`. To see available voices, run the `list_voices` query first.

**Q: Can I give my character custom documents to learn from?**
Yes! Use the `upload_knowledge_bank` tool to add files. Once uploaded, you can link them to your character using the `update_character` tool by passing the document IDs in the `docs` field.

**Q: How can I test a character's response to a specific input?**
You can use the `get_response` tool. Provide the `charID` and the user text, and the agent will return the character's generated response along with any triggered actions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convai](https://vinkius.com/mcp/convai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Convai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `convai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Convai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "convai": {
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
