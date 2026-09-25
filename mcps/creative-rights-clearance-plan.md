# Creative Rights Clearance Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-rights-clearance-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Manage creative asset permissions and generate actionable clearance workflows.

## Description
This MCP server provides a complete management system for evaluating creative asset permissions. It connects AI agents to workflows that identify missing rights, generate outreach messages for rights-holders, and track asset usage for compliance. Use `generate_clearance_plan` to evaluate alignment between permissions and intended use, `create_outreach_templates` to draft communications, `record_asset_usage` to maintain audit logs, and `get_approval_sequence` to determine the critical path for moving assets from a release hold to a released status.


## Available Tools (4)
- **create_outreach_templates**: Generates customized communication drafts for contacting rights-holders
- **record_asset_usage**: Creates a formal audit log of how an asset is being utilized
- **generate_clearance_plan**: Evaluates the alignment between existing permissions and the intended use to produce a strategic roadmap
- **get_approval_sequence**: Determines the order of operations required to move from Hold to Released status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Rights Clearance Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate my current assets and tell me what is missing for a social media campaign."

**🤖 AI Agent:**
> The clearance plan identifies that Asset ID 'IMG_001' has only Tier 2 (Restricted) clearance, which covers digital use but lacks the specific territory rights required for your global social media campaign. A release hold is active for this asset.

---

**👤 You:**
> "Generate a message to contact the rights-holder for the music track in our video."

**🤖 AI Agent:**
> Subject: Permission Request for Music Asset. Dear Rights-Holder, we are requesting permission to use your musical work for a digital advertisement on YouTube and Instagram. We will provide attribution as follows: [Attribution Preference].

---

**👤 You:**
> "What is the next step to release the assets currently on hold?"

**🤖 AI Agent:**
> The critical path requires first securing the Tier 4 (No Clearance) status for Asset 'VID_99' via the outreach template, followed by verifying the Tier 2 permissions for Asset 'IMG_42'.


## ❓ FAQ

**Q: How do I identify assets that are missing permissions?**
You can use the `generate_clearance_plan` tool. It evaluates your assets against existing permissions and flags any assets with unknown or partial authorization.

**Q: Can I automate the contact process for rights-holders?**
Yes, the `create_outreach_templates` tool generates customized communication drafts specifically designed for contacting rights-holders based on your intended use.

**Q: How can I ensure my asset usage is compliant?**
Use the `record_asset_usage` tool to create a formal audit log. This helps verify that the specific instance of use stays within the boundaries of your existing permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-rights-clearance-plan](https://vinkius.com/en/ai-agent-connect/creative-rights-clearance-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Rights Clearance Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-rights-clearance-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Rights Clearance Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-rights-clearance-plan": {
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
