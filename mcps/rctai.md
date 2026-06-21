# rct.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rctai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-apis](../categories/developer-apis.md)

Create AI-powered NPCs and metaverse scenarios — manage autonomous virtual beings and narrative logic directly from any AI agent.

## Description
Connect your AI agents to **rct.ai**, the advanced narrative engine for the gaming and metaverse industry. This MCP provides 10 tools to orchestrate autonomous virtual beings using the **Morpheus Cloud** and the **Chaos Box** algorithm.

### What you can do

- **NPC Interaction** — Send user input to NPCs and receive real-time dialogue and behavioral decisions
- **Character Lifecycle** — Create, update, and inspect AI character profiles and personalities
- **Contextual Sessions** — Manage persistent interaction sessions between players and virtual beings
- **Narrative Logic** — Configure the Chaos Box to balance stochastic randomness and scripted narrative flow

### How it works

1. Subscribe to this server
2. Sign up at [**rct.ai**](https://rct.ai/)
3. Apply for **Morpheus Cloud** developer access
4. Generate your **API Key** from the developer console
5. Configure your NPCs and integrate them into your workflow using this MCP.

### Who is this for?

- **Game Developers** — build non-linear quests and intelligent NPC interactions
- **Metaverse Architects** — create evolving virtual worlds populated by autonomous agents
- **Narrative Designers** — experiment with AI-driven storytelling and character growth


## Available Tools
- **create_character**: Create a new AI NPC profile
- **create_session**: Initialize a new interaction session
- **get_chaos_box_config**: Retrieve current Chaos Box logic parameters
- **get_character**: Get detailed configuration of a specific AI character
- **get_session**: Retrieve details about an ongoing interaction session
- **send_inference**: Send user input to an AI NPC and get a response
- **list_assets**: List assets or knowledge bases attached to characters
- **list_characters**: List all AI characters managed in your account
- **update_chaos_box_config**: Update Chaos Box decision logic parameters
- **update_character**: Update an existing AI character configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **rct.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send interaction message 'Who are you?' to NPC character 'char_123'."

**🤖 AI Agent:**
> I'm communicating with the Morpheus engine... NPC 'Guardian' (ID: char_123) responded: 'I am the keeper of the ancient scrolls. What knowledge do you seek?'. Current session status is active.

---

**👤 You:**
> "List all AI characters managed in my account."

**🤖 AI Agent:**
> Retrieving your characters... I found 3 NPCs: 1. Merchant (ID: c1), 2. Guard (ID: c2), 3. Oracle (ID: c3). All are currently 'online' in the Morpheus Cloud.

---

**👤 You:**
> "Get the current Chaos Box configuration."

**🤖 AI Agent:**
> Fetching Chaos Box parameters... Current logic is set to 'Stochastic-Balanced' with a randomness factor of 0.4. Would you like to adjust these values?


## ❓ FAQ

**Q: What is the Chaos Box and how can I configure it?**
The Chaos Box is rct.ai's proprietary narrative engine. You can use the `update_chaos_box_config` tool to adjust decision-making parameters and balance stochastic randomness within your NPC interactions.

**Q: Can I manage persistent player sessions with my AI agent?**
Yes! Use the `create_session` and `get_session` tools to maintain context and state for individual players interacting with your virtual beings.

**Q: How do I list all assets attached to my characters?**
Use the `list_assets` tool. It will retrieve all knowledge bases and data sets currently associated with your Morpheus Cloud characters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rctai](https://vinkius.com/mcp/rctai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **rct.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rctai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **rct.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rctai": {
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
