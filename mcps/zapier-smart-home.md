# Zapier Smart Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zapier-smart-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Control smart home devices via natural language through Zapier NLA API — access 5000+ app integrations for home automation.

## Description
Connect to **Zapier Natural Language Actions (NLA) API** and control your entire smart home through natural language commands across 5000+ app integrations. Turn on lights, adjust thermostats, lock doors, trigger cameras, and automate any connected device — all through simple English commands.

### What you can do

- **Natural Language Control** — Send commands like "turn on the kitchen lights" or "set thermostat to 72°F" in plain English
- **Action Discovery** — Search and discover available smart home actions across 5000+ app integrations
- **Exposed Actions** — List and manage all smart home actions you've exposed in your Zapier account
- **AI-Enabled Zaps** — List, preview, and trigger AI-enabled automation workflows (zaps)
- **Lighting Control** — Find and execute lighting actions (turn on/off, dim, color) across supported integrations
- **Climate Control** — Discover and execute thermostat and climate actions
- **Security Management** — Find and execute security, camera, and alarm actions
- **Zap Preview** — Preview automation workflows from natural language descriptions before creating them
- **Configuration** — Get setup links to expose new smart home actions for AI control

### How it works

1. Subscribe to this server
2. Enter your Zapier NLA API key (get it at https://nla.zapier.com/)
3. Start controlling your smart home with natural language from Claude, Cursor, or any MCP-compatible client

Your AI becomes a universal smart home assistant, translating your natural language commands into actions across Philips Hue, Nest, Ring, Ecobee, SmartThings, and thousands of other integrations.

### Who is this for?

- **Smart Home Owners** — control any connected device with simple natural language commands
- **Home Automation Enthusiasts** — discover and execute actions across 5000+ app integrations
- **Property Managers** — manage smart home devices across multiple properties through a unified interface
- **Accessibility Users** — control smart home devices with natural language instead of complex apps
- **Integration Builders** — build automations and workflows through Zapier's NLA API


## Available Tools
- **list_climate_actions**: List available climate/thermostat control actions
- **get_zapier_config_link**: Use this link to expose new actions for AI control.

Get the configuration link for setting up more smart home actions
- **execute_zapier_action**: Primary method for controlling devices through Zapier NLA.

Execute a specific exposed action by ID with natural language instructions
- **list_lighting_actions**: List available lighting control actions (turn on/off, dim, color)
- **list_ai_zaps**: List all AI-enabled zaps in your Zapier account
- **list_exposed_actions**: List all exposed smart home actions in your Zapier account
- **send_natural_language_command**: Zapier interprets the command and routes it to the best matching action automatically.

Send any smart home command using natural language through Zapier
- **preview_zapier_zap**: Preview a Zap from a natural language description
- **search_zapier_actions**: Returns matching actions that can be executed via the NLA API.

Search for available actions across 5000+ apps using natural language
- **list_security_actions**: List available security, camera, and alarm control actions
- **list_smarthome_actions**: Returns up to 50 matching actions that can be used for home automation.

List available smart home actions across 5000+ app integrations
- **trigger_ai_zap**: Trigger/execute a specific AI-enabled zap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zapier Smart Home** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What smart home actions do I have exposed?"

**🤖 AI Agent:**
> I found 4 exposed smart home actions in your Zapier account: 1) Turn on kitchen light (Philips Hue), 2) Set thermostat to 72°F (Nest), 3) Lock front door (August), 4) Turn off all lights (SmartThings). Would you like to execute any of these?

---

**👤 You:**
> "Search for actions to control my living room lights."

**🤖 AI Agent:**
> I found 3 lighting actions: 1) Philips Hue - Turn on Living Room Light, 2) Philips Hue - Dim Living Room Light, 3) LIFX - Set Living Room Lamp Color. You can execute any of these using their operation ID with the execute_zapier_action tool.

---

**👤 You:**
> "Turn off all the lights in the house."

**🤖 AI Agent:**
> Executing command: "turn off all the lights in the house"... Found matching action: SmartThings - Turn Off All Lights. Executing... Done! All lights have been turned off successfully.


## ❓ FAQ

**Q: What smart home devices and apps are supported through Zapier NLA?**
Zapier NLA provides access to 5000+ app integrations including Philips Hue, LIFX, Nanoleaf (lighting), Nest, Ecobee, Honeywell (climate), Ring, Arlo, SimpliSafe (security), SmartThings, Home Assistant, IFTTT, and many more. Use `search_zapier_actions` to discover specific actions for your devices.

**Q: How do I get a Zapier NLA API key?**
Visit https://nla.zapier.com/ and sign in with your Zapier account. Navigate to the NLA API settings page and generate a new API key (starts with `sk-nla-`). You'll need a Zapier account with exposed actions configured for the smart home apps you want to control.

**Q: What is the difference between exposed actions and AI zaps?**
**Exposed actions** are individual smart home actions you've configured and made available for AI execution (e.g., "turn on kitchen light"). **AI zaps** are multi-step automation workflows that can be triggered with natural language instructions. Exposed actions are for direct device control, while AI zaps are for complex workflows involving multiple steps and apps.

**Q: Can I control devices with natural language commands?**
Yes! Use the `send_natural_language_command` tool to send any smart home command in plain English. For example: "turn off all the lights", "set the thermostat to 72 degrees", or "lock the front door". The API will search for matching actions and execute the best match. You can also use `search_zapier_actions` to find specific action IDs for more precise control.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zapier-smart-home](https://vinkius.com/mcp/zapier-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zapier Smart Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zapier-smart-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zapier Smart Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zapier-smart-home": {
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
