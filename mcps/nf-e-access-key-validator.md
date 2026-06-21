# NF-e Access Key Validator MCP Server

Validate the structural integrity and compliance of Brazilian NF-e access keys.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nf-e-access-key-validator)

## Overview
**Category:** finance
**Tools Count:** 3

## Description
This MCP server provides specialized tools for verifying Brazilian Electronic Invoice (NF-e) access keys. Use `verify_key_structure` to check the 44-digit sequence for mathematical validity using the Modulo 11 algorithm. The `extract_key_metadata` tool decomposes a valid key into its constituent parts, such as CNPJ and State Code, while `validate_business_compliance` audits these components against official tax authority standards.


## Available Tools
- **extract_key_metadata**: Decomposes a valid access key into its constituent business parts for inspection
- **validate_business_compliance**: Checks if the components within a key adhere to allowed tax authority standards
- **verify_key_structure**: Determines if an access key is structurally valid based on length and the mathematical checksum


## Installation & Usage

To install and use the **NF-e Access Key Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nf-e-access-key-validator](https://vinkius.com/mcp/nf-e-access-key-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
