# shadcn/ui Dependency Resolver Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shadcnui-dependency-resolver-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [development](../categories/development.md)

Resolves exact shadcn/ui component dependencies from JSX snippets.

## Description
This MCP server solves the problem of 'dependency blindness' in AI coding agents. When an agent generates a JSX snippet using a component like ``, it often forgets that the project also requires the `dialog` component package and its associated sub-components (like `DialogContent`) to be properly installed. By using the `extract_dependencies` tool, you can provide any JSX/TSX code snippet to identify all required shadcn/ui base components and detect if essential sub-components are missing from your implementation.


## Available Tools (3)
- **extract_dependencies**: Returns required packages, count, and missing tags.

Analyzes a JSX snippet to determine required shadcn/ui components and missing sub-components
- **list_all_registry_components**: Provides a complete list of all shadcn/ui components that the server is capable of resolving
- **validate_component_registry_entry**: g., "DialogTrigger"). Returns if it is known and its base package.

Verifies if a specific string corresponds to a known shadcn/ui sub-component or base component


## 💬 Prompt Examples

Here are some examples of how you can interact with the **shadcn/ui Dependency Resolver Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this JSX: <Button>Click me</Button>"

**🤖 AI Agent:**
> The `extract_dependencies` tool identified the 'button' component as required.

---

**👤 You:**
> "Check if <DialogTrigger> is a valid shadcn component."

**🤖 AI Agent:**
> The `validate_component_registry_entry` tool confirms that 'DialogTrigger' is a known sub-component belonging to the 'dialog' base component.

---

**👤 You:**
> "List all supported shadcn components."

**🤖 AI Agent:**
> The `list_all_registry_components` tool provides the full alphabetical list of supported packages, including accordion, alert, alert-dialog, and more.


## ❓ FAQ

**Q: What does the `extract_dependencies` tool return?**
It returns a unique list of required components, the total count of detected components, and a list of any missing sub-components found in your snippet.

**Q: How does it identify components?**
The tool scans your JSX for tags starting with an uppercase letter and matches them against a strict registry of shadcn/ui component families.

**Q: Can I verify a specific tag name?**
Yes, you can use the `validate_component_registry_entry` tool to check if a specific string like 'AccordionItem' is recognized as a valid shadcn/ui component.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shadcnui-dependency-resolver-alternative](https://vinkius.com/mcp/shadcnui-dependency-resolver-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **shadcn/ui Dependency Resolver Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shadcnui-dependency-resolver-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **shadcn/ui Dependency Resolver Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shadcnui-dependency-resolver-alternative": {
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
