# Composio Smart Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/composio-smart-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Access 1000+ smart home tool integrations via Composio API — control devices through structured arguments or natural language commands.

## Description
Connect to **Composio API** and control smart home devices across 1000+ integrations through structured JSON arguments or natural language commands. Composio abstracts away authentication and API complexity, giving AI agents a unified interface to control Sensibo, Philips Hue, SmartThings, and hundreds of other smart home ecosystems.

### What you can do

- **Tool Discovery** — List and search all available smart home tools across Composio's extensive integration catalog
- **Schema Inspection** — View complete parameter schemas for any tool before executing it
- **Structured Execution** — Execute tools with precise JSON arguments matching each tool's schema
- **Natural Language Control** — Execute tools using conversational English — Composio's AI parses and maps parameters automatically
- **App-Specific Tools** — Browse all available actions for specific smart home apps like Sensibo, Philips Hue, etc.
- **Multi-Device Control** — Access tools for climate control, lighting, security, entertainment, and more
- **Unified Interface** — One API key gives access to 1000+ smart home integrations without individual auth setup

### How it works

1. Subscribe to this server
2. Enter your Composio API key (get it at https://app.composio.dev/)
3. Start controlling smart home devices from Claude, Cursor, or any MCP-compatible client

Your AI becomes a universal smart home controller, translating commands into actions across multiple device ecosystems.

### Who is this for?

- **Smart Home Enthusiasts** — control multiple device brands through a single unified interface
- **AI Agent Developers** — integrate smart home control into AI agents without managing individual API auth
- **Property Managers** — manage diverse smart home ecosystems across multiple properties
- **Automation Builders** — compose multi-device workflows using Composio's tool catalog
- **Accessibility Users** — control any connected device with simple natural language commands


## Available Tools (8)
- **execute_composio_tool**: Execute a Composio smart home tool with structured JSON arguments
- **execute_multiple_composio_tools**: Provide tool_slug with either arguments (JSON) or text (natural language) per item.

Execute multiple Composio smart home tools in a single sequential request
- **search_composio_tools**: Search for smart home tools by app slug or category keyword
- **execute_composio_tool_with_text**: Execute a Composio smart home tool using a natural language instruction
- **get_composio_tool_schema**: Retrieve the full JSON schema and accepted parameters for a specific Composio tool
- **list_app_tools**: List all available tools for a specific smart home app integration
- **list_connected_accounts**: List all connected smart home accounts and integrations in Composio
- **list_composio_tools**: List all available smart home tools and integrations in Composio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Composio Smart Home** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available smart home tools I can execute."

**🤖 AI Agent:**
> I found 150+ smart home tools available through Composio. Key categories include: Sensibo (climate control — turn on/off AC, set temperature), Philips Hue (lighting — turn on/off, dim, change color), SmartThings (hub — control devices, scenes), and many more. Use `search_composio_tools` to find tools for specific apps.

---

**👤 You:**
> "Turn on my living room AC and set it to 22°C."

**🤖 AI Agent:**
> Executing tool SENSIBO_TURN_ON with text instruction "turn on living room AC and set to 22°C"... Done! Your living room AC is now on and set to 22°C. The Sensibo device has been configured successfully.

---

**👤 You:**
> "Show me all tools available for Sensibo."

**🤖 AI Agent:**
> Found 8 Sensibo tools: SENSIBO_TURN_ON, SENSIBO_TURN_OFF, SENSIBO_SET_AC (set temperature/mode), SENSIBO_GET_AC_STATE, SENSIBO_SET_TIMER, SENSIBO_SET_SCHEDULE, SENSIBO_GET_ROOMS, SENSIBO_GET_MEASUREMENTS. You can execute any of these using `execute_composio_tool` or `execute_composio_tool_with_text`.


## ❓ FAQ

**Q: What smart home devices and apps are supported through Composio?**
Composio provides access to 1000+ smart home tool integrations including Sensibo (climate control), Philips Hue (lighting), SmartThings (hub), and many more device ecosystems. Use `list_composio_tools` to discover all available tools, or `search_composio_tools` to find tools for specific apps or categories.

**Q: What's the difference between executing a tool with arguments vs. with text?**
**With arguments** (`execute_composio_tool`): You provide a JSON object matching the tool's exact schema. This gives you precise control over every parameter. **With text** (`execute_composio_tool_with_text`): You provide natural language instructions like "turn on the AC to 72 degrees" and Composio's AI parses and maps it to the correct parameters. Use arguments for precision, text for convenience.

**Q: How do I get a Composio API key?**
Visit https://app.composio.dev/ and sign up for a Composio account. Navigate to your API settings or developer dashboard to generate an API key (starts with `ak_`). The key gives you access to all available smart home tool integrations.

**Q: Do I need separate authentication for each smart home app?**
No! Composio handles authentication to individual smart home services internally. You only need your Composio API key. However, you may need to connect your accounts to specific services through Composio's connection management first. Use the `connected_account_id` parameter when executing tools if you have multiple accounts connected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/composio-smart-home](https://vinkius.com/mcp/composio-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Composio Smart Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `composio-smart-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Composio Smart Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "composio-smart-home": {
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
