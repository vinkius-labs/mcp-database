# CNPJ Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnpj-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify the mathematical validity and structure of Brazilian CNPJ numbers.

## Description
The CNPJ Validator MCP server provides a specialized engine for verifying Brazilian business identification numbers (CNPJ) through checksum algorithms and structural analysis. It allows AI agents to perform high-precision validation of CNPJ strings without external dependencies on federal databases. Using tools like `validate_cnpj_format`, `analyze_cnpj_structure`, and `batch_validate_cnpjs`, you can confirm if a number is mathematically valid, deconstruct it into its constituent parts (root, branch, and check digits), and even infer the Brazilian state of registration based on internal regional mapping rules. This server is ideal for automating compliance checks, data cleaning, and business identification workflows within your AI-driven processes.


## Available Tools
- **analyze_cnpj_structure**: Deconstructs a CNPJ into its constituent parts
- **batch_validate_cnpjs**: Performs high-volume validation on a list of identifiers
- **validate_cnpj_format**: Validates a CNPJ string using checksum algorithm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CNPJ Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the CNPJ 12.345.678/0001-95 valid?"

**🤖 AI Agent:**
> Yes, the CNPJ 12.345.678/0001-95 is mathematically valid.

---

**👤 You:**
> "Analyze the structure of CNPJ 00.000.000/0001-91."

**🤖 AI Agent:**
> The CNPJ 00.000.000/0001-91 has a root identifier of 00000000, a branch identifier of 0001, and check digits 91. The inferred state is based on regional mapping rules.

---

**👤 You:**
> "Check if this list of CNPJs are valid: ['12345678000195', '00000000000191']"

**🤖 AI Agent:**
> Total processed: 2. Valid count: 2. Invalid count: 0.


## ❓ FAQ

**Q: Does this tool require an internet connection to the Brazilian Federal Revenue?**
No. The `validate_cnpj_format` and other tools use a local checksum algorithm (weighted summation) to verify the mathematical validity of the CNPJ without making external API calls to federal databases.

**Q: Can I validate multiple CNPJs at once?**
Yes, you can use the `batch_validate_cnpjs` tool to process an array of CNPJ strings in a single operation and receive summary statistics.

**Q: What information is returned when analyzing a CNPJ?**
By using `analyze_cnpj_structure`, you will receive the root identifier, branch identifier, check digits, and the inferred Brazilian state (UF) based on regional mapping rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnpj-validator](https://vinkius.com/mcp/cnpj-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CNPJ Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cnpj-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CNPJ Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cnpj-validator": {
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
