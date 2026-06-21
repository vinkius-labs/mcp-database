# CNPJ Validator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnpj-validator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cnpj-validator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cnpj-validator-mcp)
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


## Installation & Usage

To install and use the **CNPJ Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnpj-validator](https://vinkius.com/mcp/cnpj-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
