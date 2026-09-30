# Two-Factor Coverage Report MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/two-factor-coverage-report)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit account security posture by comparing enabled MFA methods against required security tiers.

## Description
This MCP server provides a specialized auditing suite to evaluate an account's security coverage. By analyzing the relationship between active authentication methods and assigned security priorities, it identifies critical gaps in protection. Use `get_account_security_summary` to view a high-level MFA status, `calculate_coverage_gap` to find specific deficits in security tiers, `list_available_methods` to see what a user can technically use, and `get_priority_requirements` to understand the standards for Critical, Standard, or Basic tiers.


## Available Tools (4)
- **calculate_coverage_gap**: Calculates the specific deficit between an account's enabled methods and the requirements of its assigned priority tier
- **get_account_security_summary**: Provides a high-level overview of a specific account's current multi-factor authentication (MFA) status and recovery readiness
- **get_priority_requirements**: Retrieves the definition of what constitutes "full coverage" for any given priority label
- **list_available_methods**: Identifies which second-factor methods are technically possible for a specific user based on their profile attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Two-Factor Coverage Report** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the security status for account ID 'user_123'."

**🤖 AI Agent:**
> Account 'user_123' is currently in the Standard tier. Enabled methods include Authenticator Apps. The recovery status is Fully Protected.

---

**👤 You:**
> "What is the coverage gap for account 'admin_99'?"

**🤖 AI Agent:**
> Account 'admin_99' has a coverage of 50%. The missing method is Hardware Keys, which is required for the Critical tier.

---

**👤 You:**
> "What methods are required for a Critical security tier?"

**🤖 AI Agent:**
> For the Critical tier, the required methods are Hardware Keys.


## ❓ FAQ

**Q: How is security coverage calculated?**
Coverage is calculated by comparing the number of enabled authentication methods against the total number of methods required for the account's specific security tier.

**Q: What are the different security tiers?**
There are three tiers: Critical (highest security, requires hardware keys), Standard (requires digital methods like apps or push), and Basic (allows legacy methods like SMS).

**Q: Can I see which methods are missing for a specific user?**
Yes, you can use `calculate_coverage_gap` to get a detailed breakdown of missing and unavailable methods for any given account ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/two-factor-coverage-report](https://vinkius.com/en/ai-agent-connect/two-factor-coverage-report)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Two-Factor Coverage Report** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `two-factor-coverage-report` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Two-Factor Coverage Report** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "two-factor-coverage-report": {
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
