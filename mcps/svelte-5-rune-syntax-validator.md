# Svelte 5 Rune Syntax Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/svelte-5-rune-syntax-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [development](../categories/development.md)

Ensure your Svelte components strictly adhere to the new Runes API syntax.

## Description
The Svelte 5 Rune Syntax Validator is a specialized tool for developers transitioning from Svelte 4 to Svelte 5. It performs deep structural audits of your component strings to ensure that reactive primitives like `$state`, `$derived`, `$effect`, and `$props` are used correctly. The validator enforces critical rules, such as ensuring all runes reside within `<script>` tags and verifying that `$props` follows the required destructuring pattern. By using `validate_component_syntax`, you can catch isolation breaches and boundary errors before they reach production.


## Available Tools (3)
- **rune_inventory**: Checks for the presence of required runes in a Svelte component
- **syntax_validation**: Validates the syntax of a Svelte component
- **script_boundary**: Identifies the boundaries of a script block in a Svelte component


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Svelte 5 Rune Syntax Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this Svelte 5 code valid: `<script>$state(0)</script>`?"

**🤖 AI Agent:**
> Yes, the code is valid because the `$state` rune is correctly placed within a script tag.

---

**👤 You:**
> "Check if this component has any runes: `<div>$state(true)</div>`"

**🤖 AI Agent:**
> The validator detected `$state`, but it flagged a syntax error because the rune is located outside of a script tag.

---

**👤 You:**
> "Does this snippet use props correctly: `<script>let { name } = $props();</script>`?"

**🤖 AI Agent:**
> Yes, the `$props` rune is used with a destructuring assignment, which satisfies the Svelte 5 requirement.


## ❓ FAQ

**Q: What exactly does the validator check for?**
It checks for Svelte 5 specific rules, such as ensuring `$state` is inside a script tag and that `$props` uses destructuring. You can use `validate_component_syntax` to get a detailed error report.

**Q: Can I just scan for runes without full validation?**
Yes, the `rune_inventory` tool allows you to quickly identify which runes are present in a code snippet without performing a full structural audit.

**Q: How does it handle script tag boundaries?**
The `script_boundary` tool specifically identifies the start and end of your `<script>` blocks to ensure reactive logic is properly encapsulated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/svelte-5-rune-syntax-validator](https://vinkius.com/mcp/svelte-5-rune-syntax-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Svelte 5 Rune Syntax Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `svelte-5-rune-syntax-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Svelte 5 Rune Syntax Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "svelte-5-rune-syntax-validator": {
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
