# Business Logic Gatekeeper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/business-logic-gatekeeper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Ensures code changes adhere to business invariants using regex-based validation.

## Description
The Business Logic Gatekeeper acts as a sentinel layer between code implementation and business intent. It ensures that while code may be syntactically correct, it still adheres to specific logical invariants. By using tools like `check_compliance`, `register_rule`, and `query_rules`, developers can enforce critical business truths--such as security requirements or financial integrity--directly within the development workflow. This prevents accidental violations of core logic during rapid iteration.


## Available Tools (3)
- **check_compliance**: Validates a set of file changes against the registered business rules
- **query_rules**: Retrieves a filtered list of business rules
- **register_rule**: Adds a new business rule or invariant to the gatekeeper's registry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Logic Gatekeeper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my recent changes to the payment service violate any critical rules."

**🤖 AI Agent:**
> The current changes are compliant. All critical business invariants for the payment service are satisfied.

---

**👤 You:**
> "Register a new rule for user balance integrity."

**🤖 AI Agent:**
> The rule 'user_balance_must_not_go_negative' has been successfully registered.

---

**👤 You:**
> "List all high-severity rules currently active."

**🤖 AI Agent:**
> There are 2 high-severity rules currently active in the registry.


## ❓ FAQ

**Q: How does the gatekeeper validate code?**
It uses the `check_compliance` tool to match file contents against registered `validationRegex` patterns defined in business rules.

**Q: Can I add custom business rules?**
Yes, you can use the `register_rule` tool to add new invariants with specific severity levels and affected file paths.

**Q: What is a compliance score?**
The compliance score is a value between 0 and 1 representing the ratio of satisfied rules to total applicable rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/business-logic-gatekeeper](https://vinkius.com/ai-agent-connect/business-logic-gatekeeper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Logic Gatekeeper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-logic-gatekeeper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Logic Gatekeeper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-logic-gatekeeper": {
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
