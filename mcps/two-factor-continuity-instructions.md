# Two-Factor Continuity Instructions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/two-factor-continuity-instructions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Generates safe, step-by-step recovery procedures for MFA access based on account tiers and roles.

## Description
This MCP server provides a structured framework for managing multi-factor authentication (MFA) continuity events. It allows AI agents to safely guide authorized recipients through recovery processes by identifying necessary assets and verifying governance rules. Using tools like `get_recovery_protocol` and `locate_recovery_assets`, the server provides natural language instructions on where to find recovery materials without ever exposing sensitive credentials. It is designed to bridge the gap between emergency continuity needs and secure, role-based access control.


## Available Tools (4)
- **get_recovery_protocol**: Generates a safe, step-by-step instructional guide for a specific recipient to regain access to an account
- **locate_recovery_assets**: Identifies which physical devices or storage locations need to be accessed for a recovery attempt
- **validate_recipient_eligibility**: Confirms if a specific person/role is permitted to participate in the recovery of a specific account
- **verify_release_conditions**: Checks if the necessary governance requirements are met to trigger an MFA recovery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Two-Factor Continuity Instructions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a Department Lead. What are the recovery steps for a Corporate account?"

**🤖 AI Agent:**
> To recover access to the Corporate account, first locate the encrypted USB drive in the department safe. Once retrieved, follow the standard verification protocol with your supervisor.

---

**👤 You:**
> "Where can I find the recovery assets for an Administrative account?"

**🤖 AI Agent:**
> Administrative assets are stored in the high-security dual-lock vault. You will need to coordinate with the security team to access the hardware security module.

---

**👤 You:**
> "Check if the recovery for a Personal account is authorized with the trigger 'primary_user_incapacitated'."

**🤖 AI Agent:**
> Yes, the release conditions for Personal accounts are met with the provided trigger.


## ❓ FAQ

**Q: Does this server expose actual passwords or backup codes?**
No. The server is strictly designed to provide instructions on where to find assets and how to proceed. It never returns actual passwords, secret keys, or backup codes.

**Q: How does the server determine if a user can start a recovery?**
The server uses `verify_release_conditions` to check if the required governance triggers, such as dual-authorization, have been met for the specific account category.

**Q: Can any user access Administrative accounts?**
No. Access is strictly governed by roles. You can use `validate_recipient_eligibility` to confirm if a role, such as a System Administrator, is permitted to access a specific tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/two-factor-continuity-instructions](https://vinkius.com/en/ai-agent-connect/two-factor-continuity-instructions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Two-Factor Continuity Instructions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `two-factor-continuity-instructions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Two-Factor Continuity Instructions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "two-factor-continuity-instructions": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
