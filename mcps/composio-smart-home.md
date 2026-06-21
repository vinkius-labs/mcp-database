# Composio Smart Home MCP Server

Access 1000+ smart home tool integrations via Composio API — control devices through structured arguments or natural language commands.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/composio-smart-home)

## Overview
**Category:** friends-mcp
**Tools Count:** 8

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


## Available Tools
- **execute_composio_tool**: Execute a Composio smart home tool with structured JSON arguments
- **execute_multiple_composio_tools**: Provide tool_slug with either arguments (JSON) or text (natural language) per item.

Execute multiple Composio smart home tools in a single sequential request
- **search_composio_tools**: Search for smart home tools by app slug or category keyword
- **execute_composio_tool_with_text**: Execute a Composio smart home tool using a natural language instruction
- **get_composio_tool_schema**: Retrieve the full JSON schema and accepted parameters for a specific Composio tool
- **list_app_tools**: List all available tools for a specific smart home app integration
- **list_connected_accounts**: List all connected smart home accounts and integrations in Composio
- **list_composio_tools**: List all available smart home tools and integrations in Composio


## Installation & Usage

To install and use the **Composio Smart Home** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/composio-smart-home](https://vinkius.com/mcp/composio-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
