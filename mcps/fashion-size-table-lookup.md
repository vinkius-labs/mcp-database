# Fashion Size Table Lookup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fashion-size-table-lookup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Maps physical body measurements to standardized apparel sizes across different regional sizing systems.

## Description
This MCP server provides precise apparel size recommendations by bridging the gap between physical body measurements and standardized sizing labels. Using tools like `get_size_by_measurements`, users can determine their ideal fit in various regions such as the USA or Europe. The service also allows for validating measurement accuracy via `validate_measurements` and retrieving specific dimension ranges for any given size label using `find_size_by_label`.


## Available Tools (4)
- **get_available_sizing_systems**: What regional sizing standards and gender categories does this tool support?
- **get_size_by_measurements**: Based on my body measurements, what size should I buy in a specific region's sizing system?
- **validate_measurements**: Are these physical measurements realistic and complete for the requested gender?
- **find_size_by_label**: What are the actual physical dimensions associated with a specific size label?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fashion Size Table Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on my measurements (waist: 32, hips: 40), what size should I buy in the USA for women?"

**🤖 AI Agent:**
> Based on your measurements, the recommended size in the USA is 8.

---

**👤 You:**
> "What are the dimensions for a size Medium in Europe for men?"

**🤖 AI Agent:**
> For a Men's Medium in Europe, the chest measurement range is 96-100 cm and the waist is 82-86 cm.

---

**👤 You:**
> "Are these measurements valid for a man: waist 34, chest 40?"

**🤖 AI Agent:**
> Yes, these measurements are valid and complete for the requested gender.


## ❓ FAQ

**Q: How do I know if my measurements are valid?**
You can use the `validate_measurements` tool to check if your physical dimensions are realistic and complete for your selected gender category.

**Q: Which regions are supported for sizing?**
The tool supports major sizing standards including USA and Europe. You can call `get_available_sizing_systems` to see the full list of supported regions and genders.

**Q: Can I see the specific dimensions for a size label?**
Yes, the `find_size_by_label` tool provides the exact physical measurement ranges associated with a specific size label in a given region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fashion-size-table-lookup](https://vinkius.com/en/ai-agent-connect/fashion-size-table-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fashion Size Table Lookup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fashion-size-table-lookup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fashion Size Table Lookup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fashion-size-table-lookup": {
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
