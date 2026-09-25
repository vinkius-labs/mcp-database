# Art Commission Scope Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/art-commission-scope-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms fragmented client requests into structured commission scope documents.

## Description
The Art Commission Scope Planner is a specialized toolset designed to prevent scope creep and ensure alignment between artists and clients. By using tools like `generate_scope_confirmation`, `identify_client_clarifications`, `map_approval_milestones`, and `define_handoff_and_amendment`, it converts raw requests into professional, legally-aware documents. It manages the entire lifecycle from initial inquiry to final delivery, enforcing agreed rights and change-control boundaries.


## Available Tools (4)
- **define_handoff_and_amendment**: Defines how final files are delivered and how future changes are handled
- **generate_scope_confirmation**: Generates a formal summary of the agreed-upon work to ensure alignment
- **identify_client_clarifications**: Extracts necessary questions to finalize the scope and prevent ambiguity
- **map_approval_milestones**: Creates a timeline of checkpoints to manage the creative process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Art Commission Scope Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to commission a character portrait for my book cover. I have some sketches and I need it to be high-res for print. I'll pay the agreed amount upon completion."

**🤖 AI Agent:**
> The character portrait will be a high-resolution print-ready file. We will follow the Sketch, Lineart, and Color milestones. Once the Color milestone is approved, further changes will require an amendment.

---

**👤 You:**
> "Help me clarify a request for a social media icon with personal use rights."

**🤖 AI Agent:**
> To finalize this, we need to confirm the exact dimensions for the icon and the specific social media platforms where it will be used.

---

**👤 You:**
> "Generate a scope confirmation for a logo design with full ownership rights."

**🤖 AI Agent:**
> The scope includes the design of a unique logo with full ownership transferred to the client upon final payment and delivery of the source files.


## ❓ FAQ

**Q: How does this tool prevent scope creep?**
It uses `map_approval_milestones` to establish clear checkpoints and `define_handoff_and_amendment` to set strict limits on revisions, ensuring any work outside the original agreement is handled via a formal amendment process.

**Q: Can I use this for commercial art commissions?**
Yes. The tool is designed to handle various `rightsTerms`, including Commercial and Full Ownership, ensuring the scope reflects the legal usage intended.

**Q: What happens if a client wants to change something after a milestone is approved?**
Once a milestone is signed off, any changes to that stage are considered out of scope and must be managed through the `amendmentProtocol` defined in the scope document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/art-commission-scope-planner](https://vinkius.com/en/ai-agent-connect/art-commission-scope-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Art Commission Scope Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `art-commission-scope-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Art Commission Scope Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "art-commission-scope-planner": {
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
