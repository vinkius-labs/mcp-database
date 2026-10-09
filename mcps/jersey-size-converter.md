# Jersey Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/jersey-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Converts jersey sizes between different brands and regional systems.

## Description
This MCP server provides precise jersey size transformations. It allows AI agents to map source size identifiers to equivalent target sizes using specific manufacturer or regional mapping tables. Use `list_available_systems` to find valid conversion contexts, `validate_size_format` to verify a size before conversion, and `get_size_equivalence` to perform the actual transformation.


## Available Tools (4)
- **get_size_equivalence**: Answers "What is the equivalent size in the target scale for this specific jersey?"
- **list_available_systems**: Answers "What size mapping tables (systems) are available for conversion?"
- **search_size_mappings**: Answers "What are the possible size transitions available between these two specific contexts?"
- **validate_size_format**: Answers "Is this size identifier valid and recognizable before I attempt a conversion?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jersey Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the equivalent size for a 'Large' in the Nike_US_Men system when converting to ISO_Standard_Adult?"

**🤖 AI Agent:**
> The equivalent size in the ISO_Standard_Adult system is 'L'.

---

**👤 You:**
> "Is the size 'XL' valid in the Adidas_EU_Women system?"

**🤖 AI Agent:**
> Yes, 'XL' is a valid size identifier in the Adidas_EU_Women system.

---

**👤 You:**
> "List all available size systems for the 'sports' category."

**🤖 AI Agent:**
> The available systems in the sports category are: Nike_US_Men, Adidas_EU_Men, and ISO_Standard_Adult.


## ❓ FAQ

**Q: How do I know which size systems are available?**
You can use the `list_available_systems` tool to retrieve a full registry of all valid mapping contexts and their descriptions.

**Q: Can I convert sizes between different brands?**
Yes, provided a mapping table exists between the two brands. Use `search_size_mappings` to check if a transition is defined between your source and target systems.

**Q: What happens if a size is not found in the target system?**
If the `get_size_equivalence` tool cannot find a match for the provided size within the specified system, it will return an error indicating the size is not found.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/jersey-size-converter](https://vinkius.com/en/ai-agent-connect/jersey-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jersey Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jersey-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jersey Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jersey-size-converter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
