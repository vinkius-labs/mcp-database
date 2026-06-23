# CPF/CNPJ Batch Processor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cpfcnpj-batch-processor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Validate, format, and clean Brazilian CPF and CNPJ identifiers in bulk.

## Description
The CPF/CNPJ Batch Processor is a specialized utility for handling Brazilian identification numbers. Using the `validate_batch` tool, you can verify if a list of identifiers are officially valid or duplicates. The `format_batch` tool applies standard masks (dots and dashes) to make them human-readable, while `clean_batch` strips all non-numeric characters for database readiness.


## Available Tools (3)
- **clean_batch**: Clean a batch of identifiers
- **format_batch**: 000.000-00 or 00.000.000/0000-00).

Format a batch of CPF/CNPM identifiers
- **validate_batch**: Validate a batch of CPF/CNPJ identifiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CPF/CNPJ Batch Processor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these numbers are valid: ['123.456.789-01', '00.000.000/0001-91']"

**🤖 AI Agent:**
> The validation results are: 123.456.789-01 is invalid, and 00.000.000/0001-91 is valid.

---

**👤 You:**
> "Format these raw numbers: ['12345678901', '00000000000191']"

**🤖 AI Agent:**
> The formatted numbers are: 123.456.789-01 and 00.000.000/0001-91.

---

**👤 You:**
> "Clean this list: ['123.456.789-01', '00.000.000/0001-91']"

**🤖 AI Agent:**
> The cleaned identifiers are: 12345678901 and 00000000000191.


## ❓ FAQ

**Q: How does the tool identify if a number is a CPF or CNPJ?**
The system detects the type based on the digit count: 11 digits are identified as CPF, and 1rab4 digits are identified as CNPJ.

**Q: Can I use this to clean data for a database?**
Yes, by using the `clean_batch` tool, you can strip all dots, dashes, and slashes from your identifiers, leaving only the raw numeric digits.

**Q: Does it detect duplicate numbers in a list?**
Yes, the `validate_batch` tool provides a summary that includes a count of any duplicates found within the provided batch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cpfcnpj-batch-processor](https://vinkius.com/mcp/cpfcnpj-batch-processor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CPF/CNPJ Batch Processor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cpfcnpj-batch-processor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CPF/CNPJ Batch Processor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cpfcnpj-batch-processor": {
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
