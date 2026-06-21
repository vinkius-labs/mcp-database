# NF-e Access Key Validator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nf-e-access-key-validator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nf-e-access-key-validator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nf-e-access-key-validator-mcp)
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


## Installation & Usage

To install and use the **NF-e Access Key Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nf-e-access-key-validator](https://vinkius.com/mcp/nf-e-access-key-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
