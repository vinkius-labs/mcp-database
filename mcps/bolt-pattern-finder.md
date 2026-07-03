# Bolt Pattern Finder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bolt-pattern-finder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Precise vehicle wheel specification lookup and cross-compatibility engine.

## Description
The Bolt Pattern Finder is a specialized tool for automotive enthusiasts, mechanics, and wheel retailers. It provides exact factory specifications including bolt pattern, center bore, lug nut thread size, and offset range for 99% of vehicles sold in the US, EU, and Asia over the last 30 years. Use `get_vehicle_specs` to retrieve precise hub data or `check_compatibility` to verify if wheels from one vehicle will safely fit another by comparing critical dimensions like bolt pattern and clearance.


## Available Tools (3)
- **check_compatibility**: Determines if a wheel from one vehicle will safely and functionally fit onto another vehicle
- **get_vehicle_specs**: Returns bolt pattern, center bore, lug nut thread, and offset range.

Fetches the precise factory wheel specifications for a specific vehicle
- **list_makes**: Provides a list of all supported automotive manufacturers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bolt Pattern Finder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the wheel specs for a 2015 Honda Accord?"

**🤖 AI Agent:**
> For a 2015 Honda Accord, the bolt pattern is 5x114.3mm, center bore is 64.1mm, lug nut thread size is M12x1.5, and the factory offset range is between +12mm and +52mm.

---

**👤 You:**
> "Will wheels from a 2015 Honda Accord fit a 2018 Toyota Camry?"

**🤖 AI Agent:**
> The fitment is INCOMPATIBLE. While both vehicles may share similar dimensions, the bolt pattern or center bore requirements do not match for a safe installation.

---

**👤 You:**
> "List all supported car makes."

**🤖 AI Agent:**
> The database supports a wide range of manufacturers including Acura, Audi, BMW, Chevrolet, Ford, Honda, Toyota, and many others.


## ❓ FAQ

**Q: How can I find the bolt pattern for my car?**
You can use the `get_vehicle_specs` tool by providing your vehicle's make, model, and year to get the exact bolt pattern and other hub specifications.

**Q: Can I check if my current wheels will fit a different car?**
Yes, use the `check_compatibility` tool. Provide the details of both the target vehicle and the candidate wheel to see if they are compatible based on bolt pattern, center bore, and offset.

**Q: What manufacturers are supported?**
You can retrieve a full, alphabetized list of all supported automotive manufacturers using the `list_makes` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bolt-pattern-finder](https://vinkius.com/mcp/bolt-pattern-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bolt Pattern Finder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bolt-pattern-finder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bolt Pattern Finder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bolt-pattern-finder": {
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
