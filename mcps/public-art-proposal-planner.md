# Public Art Proposal Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/public-art-proposal-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Transform fragmented art call briefs into structured submission strategies and compliance checklists.

## Description
This MCP server acts as a strategic planning engine for artists and curators navigating public art commissions. It bridges the gap between creative vision and administrative requirements by providing tools to generate strategic approaches, map necessary technical assets, organize collaborator workflows, and build chronological submission timelines. Use `generate_proposal_strategy` to align your vision with jury metrics, `map_evidence_and_assets` to identify missing documentation, and `compile_compliance_checklist` to ensure all submission rules are met before the deadline.

### Available Tools

`generate_proposal_strategy_tool`, `map_evidence_and_assets_tool`, `organize_collaborator_workflow_tool`, `construct_submission_sequence_tool`, `compile_compliance_checklist_tool`


## Available Tools (5)
- **compile_compliance_checklist_tool**: Provides a final validation tool to ensure no rules were broken
- **construct_submission_sequence_tool**: Builds a chronological timeline of actions leading up to the deadline
- **generate_proposal_strategy_tool**: Creates a high-level strategic approach to the art call
- **map_evidence_and_assets_tool**: Identifies required documentation, models, or technical drawings
- **organize_collaborator_workflow_tool**: Defines roles and commitments for various partners


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Public Art Proposal Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a call brief for a permanent park sculpture. How should I approach the strategy?"

**🤖 AI Agent:**
> To develop your strategy, please provide the full text of the call brief, the description of the park site, and the specific evaluation criteria used by the jury.

---

**👤 You:**
> "What assets do I need for a submission that requires a site photo, a 3D model, and a stability report?"

**🤖 AI Agent:**
> You will need to provide a high-resolution site photo, a digital 3D model file, and a technical stability report signed by a licensed engineer.

---

**👤 You:**
> "Check if my proposal is compliant with these requirements: [List of requirements]."

**🤖 AI Agent:**
> Your proposal is compliant with all listed requirements, though you should ensure the technical drawings are provided in the specific requested format.


## ❓ FAQ

**Q: How can I ensure my proposal meets all technical requirements?**
You can use the `map_evidence_and_assets` tool to identify every required document and the `compile_compliance_checklist` tool to verify your final submission against the original call brief. Tools available: `generate_proposal_strategy_tool`, `map_evidence_and_assets_tool`, `organize_collaborator_workflow_tool`.

**Q: Can this tool help me manage my engineering partners?**
Yes. The `organize_collaborator_workflow` tool allows you to define specific roles and deliverables for partners like structural engineers or fabricators based on the call requirements.

**Q: How do I avoid missing the submission deadline?**
Use the `construct_submission_sequence` tool. It works backward from your deadlines to create a task order and identify the critical path for your project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/public-art-proposal-planner](https://vinkius.com/en/ai-agent-connect/public-art-proposal-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Public Art Proposal Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `public-art-proposal-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Public Art Proposal Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "public-art-proposal-planner": {
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
