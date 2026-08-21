# HDB Renovation Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hdb-renovation-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Validate HDB renovation plans against structural and regulatory rules.

## Description
This MCP server provides a deterministic engine to verify if renovation actions are permitted in HDB flats. It checks structural integrity constraints, material thickness limits, and permit eligibility. Use `check_renovation_compliance` to determine if a plan is approved or rejected, `get_permitted_materials` to find technical constraints like maximum thickness, and `validate_permit_eligibility` to confirm if specific permits are required for your flat type.


## Available Tools (3)
- **get_permitted_materials**: Retrieves the technical constraints and requirements for specific renovation materials
- **check_renovation_compliance**: Determines if a specific renovation plan is legal and safe
- **validate_permit_eligibility**: Checks if a specific permit can be applied for based on the flat's characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HDB Renovation Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it okay to hack a structural wall in a 4-room flat?"

**🤖 AI Agent:**
> No, hacking a structural wall is strictly prohibited and will result in a REJECT status.

---

**👤 You:**
> "What are the rules for installing wooden flooring in a 5-room flat?"

**🤖 AI Agent:**
> The installation is approved with conditions: you must use an HDB-approved contractor and the flooring must not exceed 8mm in thickness.

---

**👤 You:**
> "Can I apply for an NEA Noise Permit for my 3-room flat?"

**🤖 AI Agent:**
> Yes, a 3-room flat is eligible to apply for the NEA Noise Permit.


## ❓ FAQ

**Q: Can I hack a wall in my HDB flat?**
It depends on the wall type. You can hack non-structural walls, but hacking a structural wall will result in a REJECT status via `check_renovation_compliance`.

**Q: How do I know if my flooring is allowed?**
Use the `get_permitted_materials` tool to check the maximum allowed thickness and whether an approved contractor is required for your specific material.

**Q: Do I need a permit for my renovation?**
You can use `validate_permit_eligibility` to check if your flat type is eligible for specific permits like the HDB Renovation Permit or NEA Noise Permit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hdb-renovation-compliance-checker](https://vinkius.com/ai-agent-connect/hdb-renovation-compliance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HDB Renovation Compliance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hdb-renovation-compliance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HDB Renovation Compliance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hdb-renovation-compliance-checker": {
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
