# Creative Archive Legacy Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-archive-legacy-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legacy-management](../categories/legacy-management.md)

Transform creative assets and personal wishes into structured stewardship, access, and succession plans.

## Description
This MCP server provides a suite of tools to manage a creator's legacy. It allows for the generation of comprehensive stewardship plans, the definition of authorized access instructions, the drafting of physical documentation tasks, the mapping of future decision points, and the preparation of structured review agendas. Use `generate_stewardship_plan` to define management strategies, `create_access_instructions` to manage succession contacts, `draft_documentation_actions` for organizational preservation, `map_future_decision_points` to track review horizons, and `generate_review_agenda` to guide executors through periodic evaluations.


## Available Tools (5)
- **create_access_instructions**: Define how authorized individuals can interact with the works
- **draft_documentation_actions**: List the non-digital organizational steps required to preserve the legacy
- **generate_review_agenda**: Prepare a structured meeting guide for executors and successors
- **generate_stewardship_plan**: Create a comprehensive management strategy for the creative estate
- **map_future_decision_points**: Identify specific moments in the future where the estate must make significant choices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Archive Legacy Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me create a stewardship plan for my art collection."

**🤖 AI Agent:**
> I have generated a stewardship strategy that prioritizes active curation while maintaining strict privacy for unreleased sketches.

---

**👤 You:**
> "How can I prepare for my next legacy review meeting?"

**🤖 AI Agent:**
> I have prepared a structured agenda including discussion topics for verifying access permissions and a list of required attendees.

---

**👤 You:**
> "What are the next steps for organizing my physical records?"

**🤖 AI Agent:**
> The recommended actions include labeling existing physical files and updating the central registry to align with your stewardship philosophy.


## ❓ FAQ

**Q: How do I create a management strategy for my work?**
You can use the `generate_stewardship_plan` tool to synthesize your stewardship preferences, privacy boundaries, and display intentions into a cohesive strategy.

**Q: Can I define who has access to my creative assets?**
Yes, the `create_access_instructions` tool allows you to define authorization rules and a contact directory for your designated succession contacts.

**Q: Does this tool handle digital file storage?**
No, the `draft_documentation_actions` tool focuses on non-digital organizational steps like cataloging and physical preservation needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-archive-legacy-plan](https://vinkius.com/en/ai-agent-connect/creative-archive-legacy-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Archive Legacy Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-archive-legacy-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Archive Legacy Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-archive-legacy-plan": {
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
