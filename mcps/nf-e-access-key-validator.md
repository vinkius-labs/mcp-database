# NF-e Access Key Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nf-e-access-key-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Validate the structural integrity and compliance of Brazilian NF-e access keys.

## Description
This MCP server provides specialized tools for verifying Brazilian Electronic Invoice (NF-e) access keys. Use `verify_key_structure` to check the 44-digit sequence for mathematical validity using the Modulo 11 algorithm. The `extract_key_metadata` tool decomposes a valid key into its constituent parts, such as CNPJ and State Code, while `validate_business_compliance` audits these components against official tax authority standards.


## Available Tools
- **extract_key_metadata**: Decomposes a valid access key into its constituent business parts for inspection
- **validate_business_compliance**: Checks if the components within a key adhere to allowed tax authority standards
- **verify_key_structure**: Determines if an access key is structurally valid based on length and the mathematical checksum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NF-e Access Key Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this NF-e key valid: 3523100000000000015555001000000001?"

**🤖 AI Agent:**
> The access key is structurally valid and passes the Modulo 11 checksum.

---

**👤 You:**
> "Extract information from this key: 3523100000000000015555001000000001"

**🤖 AI Agent:**
> The extracted metadata includes State Code: 35, CNPJ: 23100000000000, Model: 55, Series: 001, Number: 000000001, and Emission Type: 1.

---

**👤 You:**
> "Check if this key follows tax standards: 3523100000000000015555001000000001"

**🤖 AI Agent:**
> The key is compliant with all checked regulatory standards.


## ❓ FAQ

**Q: What does `verify_key_structure` do?**
It checks if the 44-digit sequence is purely numeric, exactly 44 digits long, and passes the Modulo 11 checksum verification.

**Q: How can I see the issuer's details?**
Use the `extract_key_metadata` tool. It will parse the key and return the CNPJ, State Code, and other relevant metadata.

**Q: Does this tool check for tax compliance?**
Yes, the `validate_business_compliance` tool audits components like Model and Emission Type against official regulatory catalogs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nf-e-access-key-validator](https://vinkius.com/mcp/nf-e-access-key-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NF-e Access Key Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nf-e-access-key-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NF-e Access Key Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nf-e-access-key-validator": {
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
