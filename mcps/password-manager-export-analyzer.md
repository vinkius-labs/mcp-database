# Password Manager Export Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/password-manager-export-analyzer)
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


## ❓ FAQ

**Q: Does the AI see my passwords?**
NEVER. Passwords are masked as '••••••••'. Only aggregate stats are sent.

**Q: Which managers are supported?**
Any CSV export: Bitwarden, LastPass, 1Password, KeePass, Dashlane.

**Q: Should I delete the CSV after?**
Yes! Always delete unencrypted exports after analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-manager-export-analyzer](https://vinkius.com/mcp/password-manager-export-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Password Manager Export Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `password-manager-export-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Password Manager Export Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "password-manager-export-analyzer": {
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
