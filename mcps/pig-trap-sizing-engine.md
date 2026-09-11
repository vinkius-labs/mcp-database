# Pig Trap Sizing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pig-trap-sizing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates precise dimensions for pig trap barrels and kicker lines.

## Description
This MCP server provides technical calculation tools for sizing pig trap launchers and receivers. It determines required barrel diameter and length, calculates optimal kicker line sizes, and validates pig compatibility based on pipeline geometry and pig type. Use `get_sizing_summary` to generate a complete specification package for new installations, or `validate_pig_compatibility` to check if existing equipment can safely house specific cleaning, intelligent, or batching pigs.


## Available Tools (4)
- **get_kicker_line_size**: Calculates the optimal diameter for the kicker line to ensure effective pig movement
- **get_barrel_dimensions**: Determines the required internal diameter and length of a pig trap barrel
- **get_sizing_summary**: Provides a complete sizing package for a single pig trap installation
- **validate_pig_compatibility**: Checks if a specific pig can safely fit within a predefined trap setup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pig Trap Sizing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a full sizing specification for a new trap. The pipeline is 24 inches, the pig is 15 feet long, the pig diameter is 23.5 inches, and it is an intelligent pig."

**🤖 AI Agent:**
> The required barrel diameter is 24 inches, the barrel length is 22.5 feet, and the recommended kicker line diameter is 4 inches.

---

**👤 You:**
> "Will a 12-foot cleaning pig fit in my existing 15-foot barrel that has a 12-inch diameter? The pipeline is 10 inches."

**🤖 AI Agent:**
> Yes, the pig is compatible with the existing trap setup.

---

**👤 You:**
> "What is the best kicker line size for a 30-inch pipeline using a batching pig?"

**🤖 AI Agent:**
> The recommended kicker line diameter for a 30-inch pipeline with a batching pig is 6 inches.


## ❓ FAQ

**Q: How do I calculate the full specifications for a new trap?**
You can use the `get_sizing_summary` tool. Provide the pipeline diameter, pig length, pig diameter, and the pig type to receive a complete package including barrel and kicker line dimensions.

**Q: Can I check if my current barrel is large enough for an intelligent pig?**
Yes. Use the `validate_pig_compatibility` tool by providing the existing barrel dimensions and the specific dimensions and type of the intelligent pig.

**Q: What pig types are supported?**
The engine supports cleaning, intelligent, and batching pigs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pig-trap-sizing-engine](https://vinkius.com/en/ai-agent-connect/pig-trap-sizing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pig Trap Sizing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pig-trap-sizing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pig Trap Sizing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pig-trap-sizing-engine": {
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
