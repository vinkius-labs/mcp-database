# Password Manager Export Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/password-manager-export-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/password-manager-export-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/password-manager-export-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyze Bitwarden, LastPass, or 1Password CSV exports for weak and duplicate passwords — without EVER sending real passwords to the AI.

## Description
This engine performs a local security audit. It auto-detects password columns, calculates stats (avg length, duplicates, weak entries), and sends ONLY masked data to the AI.

### The Superpowers

- **Military-Grade Privacy:** Passwords are NEVER sent to the LLM.
- **Universal Support:** Bitwarden, LastPass, 1Password, KeePass.
- **Actionable Report:** Weak, duplicate, and empty passwords identified instantly.


## Available Tools
- **analyze_password_export**: The tool analyzes password strength and duplicates WITHOUT ever transmitting real passwords.

Analyze a password manager CSV export (Bitwarden, LastPass, 1Password) for security vulnerabilities. NEVER sends actual passwords to the AI — only aggregate statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Password Manager Export Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many duplicate passwords do I have?"

**🤖 AI Agent:**
> You have 23 duplicate groups across 142 accounts. 8 passwords are weak (<8 chars).

---

**👤 You:**
> "Which sites have the most accounts?"

**🤖 AI Agent:**
> google.com (5), github.com (3), amazon.com (3).

---

**👤 You:**
> "Any accounts with empty passwords?"

**🤖 AI Agent:**
> 4 entries have empty passwords. Likely SSO accounts.


## Installation & Usage

To install and use the **Password Manager Export Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-manager-export-analyzer](https://vinkius.com/mcp/password-manager-export-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
