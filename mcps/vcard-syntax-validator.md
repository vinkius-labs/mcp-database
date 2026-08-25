# vCard Syntax Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vcard-syntax-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic parser and validator for vCard (VCF) strings.

## Description
This MCP server provides precise parsing and validation for vCard (VCF) strings across versions 2.1, 3.0, and 4.0. It ensures structural integrity by verifying `BEGIN:VCARD` and `END:VCARD` encapsulation, checking for required identity fields like `FN` and `N`, and validating parameter syntax. Use `parse_vcard_structure` to verify the overall validity and version, `extract_property_values` to retrieve clean data, and `validate_parameter_syntax` to detect malformed property parameters.


## Available Tools (3)
- **extract_property_values**: Retrieves the clean key-value pairs from a valid vCard, accounting for parameter stripping
- **validate_parameter_syntax**: Checks the integrity of parameters attached to specific properties to ensure they are not malformed
- **parse_vcard_structure**: Validates the fundamental structure of a vCard string and checks for encapsulation and required identity fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vCard Syntax Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this vCard valid: 'BEGIN:VCARD\nFN:John Doe\nEND:VCARD'?"

**🤖 AI Agent:**
> Yes, the vCard is valid and uses version 2.1.

---

**👤 You:**
> "Check if the parameters for the TEL property are correct in this vCard."

**🤖 AI Agent:**
> The parameters for the TEL property are syntactically correct.

---

**👤 You:**
> "Extract the email address from this vCard string."

**🤖 AI Agent:**
> john.doe@vinkius.com


## ❓ FAQ

**Q: Which vCard versions are supported?**
The server supports vCard versions 2.1, 3.0, and 4.0.

**Q: How can I check if a vCard is missing required fields?**
You can use the `parse_vcard_structure` tool, which returns a list of `missingRequiredProperties` if identity fields like `FN` or `N` are absent.

**Q: Can I extract specific values like phone numbers?**
Yes, use the `extract_property_values` tool and specify the `targetKey` (e.g., 'TEL') to get the clean values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vcard-syntax-validator](https://vinkius.com/ai-agent-connect/vcard-syntax-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **vCard Syntax Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vcard-syntax-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **vCard Syntax Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vcard-syntax-validator": {
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
