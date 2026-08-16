# Tailwind v4 Theme Variable Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tailwind-v4-theme-variable-extractor-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extracts CSS variables from Tailwind v4 @theme blocks.

## Description
This MCP server provides a specialized engine for parsing Tailwind CSS v4 configuration. It isolates the @theme block within your CSS and extracts all defined CSS variables, such as --color-primary or --spacing-sm. By using the extract_tailwind_variables tool, you can instantly retrieve a structured list of variables categorized by type, including colors, spacing, and fonts. This is essential for agents working with modern Tailwind v4 projects where configuration has moved from JavaScript to CSS.


## Available Tools (1)
- **extract_tailwind_variables**: The tool will isolate the block and return all extracted variables, their count, and the categories found.

Extracts CSS variables from a Tailwind v04 @theme block


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailwind v4 Theme Variable Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract variables from this CSS: @theme { --color-primary: #000; --spacing-md: 1rem; }"

**🤖 AI Agent:**
> { "extractedVariables": {"--color-primary": "#000", "--spacing-md": "1rem"}, "totalCount": 2, "categoriesFound": ["color", "spacing"] }

---

**👤 You:**
> "What variables are in this @theme block?"

**🤖 AI Agent:**
> The extracted variables include --color-primary, --spacing-md, and --font-sans.

---

**👤 You:**
> "Can you find all color variables in my CSS?"

**🤖 AI Agent:**
> I found 3 color variables: --color-red-500, --color-blue-500, and --color-green-500.


## ❓ FAQ

**Q: What does this tool do?**
It parses a CSS string to find the @theme block and extracts all variables like --color-blue-500.

**Q: Does it support Tailwind v3?**
No, this tool is specifically designed for the new @theme block syntax introduced in Tailwind CSS v4.

**Q: How can I use it with Cursor or Claude Desktop?**
You can connect via Vinkius Edge using your personal Connection Token. Once connected, you can simply ask the agent to extract variables from a CSS snippet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tailwind-v4-theme-variable-extractor-alternative](https://vinkius.com/ai-agent-connect/tailwind-v4-theme-variable-extractor-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailwind v4 Theme Variable Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailwind-v4-theme-variable-extractor-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailwind v4 Theme Variable Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailwind-v4-theme-variable-extractor-alternative": {
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
