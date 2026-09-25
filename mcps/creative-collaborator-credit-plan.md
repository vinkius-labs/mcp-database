# Creative Collaborator Credit Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-collaborator-credit-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage complex attribution and credit workflows for creative projects.

## Description
This MCP server provides a structured framework for managing contributor attribution. It reconciles contributor inputs, prior agreements, and explicit consent to generate accurate credit proposals. Use `generate_credit_proposal` to draft layouts, `create_confirmation_workflow` to manage approval steps, and `finalize_attribution_record` to lock in the final credit structure. For handling conflicts, `get_disagreement_resolution_agenda` provides a mediation roadmap, while `get_outlet_specific_actions` adapts credits for different media formats.


## Available Tools (5)
- **finalize_attribution_record**: Lock in the credit structure and create a formal record of the attribution
- **generate_credit_proposal**: Create a drafted layout of how contributors should be credited
- **get_disagreement_resolution_agenda**: Provide a structured roadmap for handling conflicts
- **get_outlet_specific_actions**: Identify technical or formatting changes needed for a specific medium
- **create_confirmation_workflow**: Generate the steps required to move from a proposal to a finalized attribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Collaborator Credit Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a credit proposal for a project with three contributors: Alice (Lead Designer), Bob (Illustrator), and Charlie (Technical Architect), following alphabetical order."

**🤖 AI Agent:**
> The proposed credit list is: Alice (Lead Designer), Bob (Illustrator), and Charlie (Technical Architect).

---

**👤 You:**
> "What are the steps to finalize the attribution for a digital publication?"

**🤖 AI Agent:**
> The workflow includes verifying individual consent and performing a final proofreading for digital formats.

---

**👤 You:**
> "How can I resolve a dispute regarding the role description of a contributor?"

**🤖 AI Agent:**
> You should use the disagreement resolution agenda to mediate the role-description-dispute by reviewing prior agreements.


## ❓ FAQ

**Q: How does the tool handle conflicting credit requests?**
You can use `get_disagreement_resolution_agenda` to generate a structured mediation roadmap that references existing `priorAgreements` and current `consentStatus` to resolve disputes.

**Q: Can I change the credit list after it is finalized?**
No. Once `finalize_attribution_record` is executed, the record is immutable. Any changes require generating a new proposal and a new record.

**Q: How do I prepare credits for a specific publication like a book or a website?**
Use `get_outlet_specific_actions` with your finalized record ID to receive technical instructions and formatting requirements for your target outlet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-collaborator-credit-plan](https://vinkius.com/en/ai-agent-connect/creative-collaborator-credit-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Collaborator Credit Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-collaborator-credit-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Collaborator Credit Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-collaborator-credit-plan": {
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
