# Account Recovery Readiness Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/account-recovery-readiness-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Evaluates user account security profiles to identify recovery vulnerabilities and prioritized remediation steps.

## Description
This MCP server provides specialized auditing tools to assess how prepared a user is for account lockout scenarios. By analyzing existing recovery vectors like email, phone, and hardware keys, it identifies critical gaps in security. Use `audit_account_readiness` to get a full readiness score and status, or `calculate_readiness_gap` to compare current settings against a target security profile. It helps ensure accounts have the necessary redundancy across different verification methods.


## Available Tools (4)
- **audit_account_readiness**: Evaluates a specific user account to determine its current recovery readiness and identify gaps
- **calculate_readiness_gap**: Compares a set of existing factors against a target security profile to quantify the "gap."
- **get_factor_requirements**: Retrieves the standard definitions and required characteristics for each recovery factor type
- **list_user_recovery_factors**: Provides a raw inventory of all recovery methods currently linked to a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Account Recovery Readiness Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you audit the readiness for account ID user_123?"

**🤖 AI Agent:**
> The audit for user_123 shows a status of 'At Risk' with a score of 45. Missing factors include 'security_key' and 'backup_codes'. It is highly recommended to set up a hardware security key immediately.

---

**👤 You:**
> "What are the requirements for a security key factor?"

**🤖 AI Agent:**
> A security key is a high-importance, high-risk factor that provides phishing-resistant, hardware-based authentication for account recovery.

---

**👤 You:**
> "Calculate the gap between these factors: ['recovery_email'] and ['recovery_email', 'backup_codes', 'security_key']."

**🤖 AI Agent:**
> The gap score is 2. The missing factors are 'backup_codes' and 'security_key'. You should prioritize adding a security key first.


## ❓ FAQ

**Q: What does the readiness score represent?**
The score is a numerical value representing the strength of the recovery profile based on the diversity and security of configured factors.

**Q: How can I see which recovery methods a user has configured?**
You can use the `list_user_recovery_factors` tool to retrieve a raw inventory of all recovery methods currently linked to a specific account.

**Q: What is the difference between hard and soft recovery factors?**
Hard factors, like Security Keys, provide autonomous, high-security recovery. Soft factors, like Recovery Email, rely on external infrastructure or human interaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/account-recovery-readiness-audit](https://vinkius.com/en/ai-agent-connect/account-recovery-readiness-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Account Recovery Readiness Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `account-recovery-readiness-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Account Recovery Readiness Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "account-recovery-readiness-audit": {
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
