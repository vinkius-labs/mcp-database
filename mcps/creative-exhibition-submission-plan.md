# Creative Exhibition Submission Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-exhibition-submission-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

An intelligent decision-support engine that evaluates artist works against exhibition calls to generate actionable submission strategies.

## Description
This MCP server provides a suite of specialized tools to help artists navigate the complexities of exhibition submissions. Use `evaluate_submission_eligibility` to check if works meet technical and thematic requirements, `generate_asset_checklist` to prepare necessary files and materials, `verify_rights_and_permissions` to protect intellectual property, and `create_submission_roadmap` to build a professional timeline for deadlines. It bridges the gap between creative intent and logistical execution.


## Available Tools (4)
- **generate_asset_checklist**: Identifies exactly what files, physical materials, or documentation must be prepared
- **create_submission_roadmap**: Builds a chronological timeline of tasks and communication steps to ensure a professional submission
- **evaluate_submission_eligibility**: Determines if a specific work meets the hard constraints of an exhibition call and the user's personal criteria
- **verify_rights_and_permissions**: Analyzes the legal implications of the submission to ensure the artist is not signing away unfavorable rights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Exhibition Submission Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I submit my 'Neon Dreams' sculpture to the upcoming City Gallery call?"

**🤖 AI Agent:**
> Based on the City Gallery requirements, your 'Neon Dreams' sculpture meets the medium constraints, but you will need to prepare a technical rider for the installation.

---

**👤 You:**
> "What do I need to prepare for the Museum of Modern Art submission?"

**🤖 AI Agent:**
> You need to prepare high-resolution digital images (300dpi), a signed artist statement, and a detailed CV.

---

**👤 You:**
> "Create a timeline for my submission due on December 1st."

**🤖 AI Agent:**
> To meet the December 1st deadline, you should finalize your asset checklist by November 15th and complete all shipping logistics by November 25th.


## ❓ FAQ

**Q: How does the tool evaluate if my work is suitable?**
The `evaluate_submission_eligibility` tool compares your candidate works against the specific themes, technical constraints, and deadlines provided in the exhibition call.

**Q: Can I use this to prepare my technical files?**
Yes, you can use `generate_asset_checklist` to identify exactly which high-resolution images, documentation, or physical assets are required for a specific call.

**Q: Does this help with legal concerns?**
Yes, the `verify_rights_and_permissions` tool analyzes the legal terms of an exhibition call to ensure they align with your intellectual property preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-exhibition-submission-plan](https://vinkius.com/en/ai-agent-connect/creative-exhibition-submission-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Exhibition Submission Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-exhibition-submission-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Exhibition Submission Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-exhibition-submission-plan": {
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
