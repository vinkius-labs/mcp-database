# Import Order Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/import-order-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enforce deterministic import ordering and detect unused imports using AST analysis.

## Description
The Import Order Enforcer uses Abstract Syntax Tree (AST) parsing to ensure your source files maintain a consistent structure. It validates that imports are correctly grouped into categories like 'builtin', 'external', and 'internal' while enforcing alphabetical sorting within each group. Use the `validate_import_compliance` tool to check for grouping or spacing violations, `detect_unused_imports` to identify dead code, and `generate_fixed_import_block` to automatically reconstruct a clean import section.


## Available Tools (3)
- **detect_unused_imports**: Detects unused imports
- **fix_imports**: Generates a fixed import block
- **validate_imports**: Validates import compliance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Import Order Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any unused imports in this code? 
import { useState, useEffect } from 'react';
import { data } from './utils';
const x = 10;"

**🤖 AI Agent:**
> The following imports are unused: 'useState' at line 1, 'useEffect' at line 1.

---

**👤 You:**
> "Check if my imports follow the rules for this file: 
import { z } from 'zod';
import fs from 'fs';"

**🤖 AI Agent:**
> The import order is valid according to your configuration.

---

**👤 You:**
> "Fix the imports in this block: 
import { b } from 'pkg-b';
import { a } from 'pkg-a';"

**🤖 AI Agent:**
> import { a } from 'pkg-a';
import { b } from 'pkg-b';


## ❓ FAQ

**Q: How can I find unused imports in my file?**
Use the `detect_unused_imports` tool by providing your file content; it will return a list of all identifiers that are declared but never used.

**Q: Can this tool fix my import order automatically?**
Yes, the `generate_fixed_import_block` tool analyzes your current imports and returns a perfectly formatted block following your specified rules.

**Q: Does it support custom groups?**
Yes, you can define specific grouping logic for 'builtin', 'external', 'internal', 'parent', and 'sibling' paths.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/import-order-enforcer](https://vinkius.com/mcp/import-order-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Import Order Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `import-order-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Import Order Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "import-order-enforcer": {
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
