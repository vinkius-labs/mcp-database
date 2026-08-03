# React Server Action Route Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/react-server-action-route-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extracts Next.js Server Actions and maps them to deterministic API routes.

## Description
The React Server Action Route Mapper bridges the gap between your Next.js application logic and AI agents. By scanning JSX strings for `use server` directives, it identifies exported asynchronous functions and generates permanent, deterministic route identifiers using a bitwise hashing algorithm. This prevents AI agents from hallucinating incorrect fetch calls to internal endpoints by providing a reliable map of available actions via `map_server_actions`. You can also use `validate_component_syntax` to ensure your code is structurally sound before scanning, or `preview_route_hash` to test how specific function names will be transformed into IDs.


## Available Tools (3)
- **validate_component_syntax**: Validates the structural syntax of a JSX string
- **map_server_actions**: Maps server actions found in a JSX string
- **preview_route_hash**: Previews a route hash for a given input string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **React Server Action Route Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have this Next.js file: `export async function updateProfile(data) { 'use server'; ... }`. What is the route ID?"

**🤖 AI Agent:**
> The identified action is `updateProfile` and its generated route ID is `a1b2c3d4`.

---

**👤 You:**
> "Check if this code snippet is valid for scanning: `const x = 10; function test() {}`"

**🤖 AI Agent:**
> The syntax validation returned `isValid: true`, meaning the structure is sound enough for regex scanning.

---

**👤 You:**
> "What happens if I use `preview_route_hash` with the string 'submitForm'?"

**🤖 AI Agent:**
> The tool will generate the deterministic hash for 'submitForm', which is `e5f6g7h8`.


## ❓ FAQ

**Q: How does the tool identify a Server Action?**
The tool scans for the `use server` directive within the provided JSX string. Only exported asynchronous functions found in files containing this directive are mapped.

**Q: Is the generated route ID permanent?**
Yes. The mapping is strictly deterministic using a bitwise transformation algorithm. As long as the function name remains unchanged, the `generatedRouteId` will remain identical.

**Q: Can I test a hash without scanning a whole file?**
Yes, you can use the `preview_route_hash` tool to input a specific string and see exactly what hexadecimal ID it will produce.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/react-server-action-route-mapper](https://vinkius.com/mcp/react-server-action-route-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **React Server Action Route Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `react-server-action-route-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **React Server Action Route Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "react-server-action-route-mapper": {
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
