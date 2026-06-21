# rct.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rctai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rctai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rctai-mcp)
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


## Installation & Usage

To install and use the **rct.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rctai](https://vinkius.com/mcp/rctai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
