# License Header Injector and Verifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/license-header-injector-and-verifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enforce, audit, and repair mandatory copyright headers in source files.

## Description
This MCP server provides tools to ensure legal compliance by managing file headers. Use `apply_license_header` to automatically prepend missing copyright templates, `identify_header_drift` to detect formatting discrepancies, and `validate_template_integrity` to verify your template structure. It handles inspection windows and year agnosticism for auditing.


## Available Tools (3)
- **validate_template_integrity**: Ensures the provided template is a valid, usable copyright block
- **apply_license_header**: Checks if a file is compliant and prepends the header if missing
- **identify_header_drift**: Detects when a header exists but contains incorrect characters, spacing, or formatting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **License Header Injector and Verifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this file has the correct license header: 'Copyright 2024 Vinkius'"

**🤖 AI Agent:**
> The file is compliant with the required copyright notice.

---

**👤 You:**
> "Is there any drift in my copyright template?"

**🤖 AI Agent:**
> No structural discrepancies were found in the template.

---

**👤 You:**
> "Verify if my template is valid for use."

**🤖 AI Agent:**
> The template meets all structural requirements and is ready for deployment.


## ❓ FAQ

**Q: How does the tool handle different years in the copyright notice?**
The system uses Year Agnosticism to recognize valid headers even if the numerical year differs from the template.

**Q: What happens if a header is missing?**
The `apply_license_header` tool follows the Injection Protocol to prepend the template and a newline to the file.

**Q: Can I detect spacing errors in my header?**
Yes, `identify_header_drift` flags any deviation from the Strict Structural Match, including punctuation and spacing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/license-header-injector-and-verifier](https://vinkius.com/mcp/license-header-injector-and-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **License Header Injector and Verifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `license-header-injector-and-verifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **License Header Injector and Verifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "license-header-injector-and-verifier": {
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
