# Accessible Household Support Agreement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-household-support-agreement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates personalized, consent-driven household management plans.

## Description
This MCP server provides a framework for creating personalized household management plans. It ensures that all support is provided within explicit user-defined boundaries. Users can define support tasks, independence zones, and availability windows. The server uses `validate_consent_permission` to ensure every assistance request respects established limits, `generate_support_agreement` to produce clear documentation, `get_communication_and_backup_plan` for logistical coordination, and `create_review_agenda` to facilitate periodic reviews of the agreement.


## Available Tools (4)
- **generate_support_agreement**: Creates the core plain-language support agreement document
- **create_review_agenda**: Produces a structured meeting outline for agreement reviews
- **get_communication_and_backup_plan**: Generates logistical details for communication and backup coverage
- **validate_consent_permission**: Verifies if a task is permissible under current consent boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Household Support Agreement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a support agreement for a household with two members, including meal prep and cleaning, while keeping laundry as an independent task."

**🤖 AI Agent:**
> Support Agreement: Household members are Member A and Member B. Supported tasks include meal prep and cleaning. Independent tasks include laundry. All support will be provided within the specified consent boundaries.

---

**👤 You:**
> "Is it okay to request physical assistance for cleaning if my boundary is 'verbal guidance only'?"

**🤖 AI Agent:**
> No, the requested task violates your defined boundary of 'verbal guidance only'.

---

**👤 You:**
> "Create a review agenda for our next meeting on October 15th."

**🤖 AI Agent:**
> Review Agenda for October 15th: 1. Boundary Check (verifying consent limits), 2. Autonomy Check (verifying independence needs).


## ❓ FAQ

**Q: How does the server ensure my boundaries are respected?**
The server uses the `validate_consent_permission` tool to check every requested task against your defined consent boundaries before any plan is finalized.

**Q: Can I specify tasks I want to do alone?**
Yes, you can define independence zones through the support agreement process to ensure your autonomy is maintained.

**Q: What happens if the primary support person is unavailable?**
You can define a contingency protocol using the `get_communication_and_backup_plan` tool to establish clear backup coverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-household-support-agreement](https://vinkius.com/en/ai-agent-connect/accessible-household-support-agreement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Household Support Agreement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-household-support-agreement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Household Support Agreement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-household-support-agreement": {
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
