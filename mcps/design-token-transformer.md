# Design Token Transformer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/design-token-transformer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert, resolve, and generate multi-platform design tokens (JSON, CSS, SCSS, Tailwind, etc.).

## Description
A specialized utility for converting, resolving, and generating multi-platform design tokens across various CSS, mobile, and design tool formats. Use `transform_tokens` to convert between syntaxes like JSON and Tailwind while resolving all internal aliases to their primitive values. Use `generate_dark_mode_tokens` to create dark mode themes by adjusting OKLCH lightness for visual consistency. Additionally, use `generate_color_scale` to produce a complete 50-950 color weight scale from three anchor colors.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Design Token Transformer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert these JSON tokens to CSS: {"color": {"primary": "#007bff"}}"

**🤖 AI Agent:**
> :root { --color-primary: #007bff; }

---

**👤 You:**
> "Generate a color scale using #f8f9fa, #6c757d, and #212529 as anchors."

**🤖 AI Agent:**
> {"50": "#f8f9fa", "100": "#f1f3f5", "200": "#e9ecef", "300": "#dee2e6", "400": "#ced4da", "500": "#adb5bd", "600": "#6c757d", "700": "#495057", "800": "#343a40", "900": "#212529", "950": "#1a1d20"}

---

**👤 You:**
> "Generate dark mode tokens from this JSON: {"color": {"primary": "#007bff"}}"

**🤖 AI Agent:**
> {"color": {"primary": "#004a99"}}


## ❓ FAQ

**Q: How can I convert tokens from JSON to Tailwind?**
Use the `transform_tokens` tool, specifying 'json' as your `sourceFormat` and 'tailwind' as your `targetFormat`. Tools available: `your_tool_name`.

**Q: Can this tool handle color aliases?**
Yes, the `transform_tokens` tool automatically resolves all internal references and aliases to their primitive values during transformation.

**Q: How do I generate a dark mode theme?**
Use the `generate_dark_mode_tokens` tool with your existing light-mode JSON token data. It uses OKLCH lightness inversion for visual consistency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/design-token-transformer](https://vinkius.com/mcp/design-token-transformer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Design Token Transformer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `design-token-transformer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Design Token Transformer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "design-token-transformer": {
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
