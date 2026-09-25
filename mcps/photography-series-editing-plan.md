# Photography Series Editing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photography-series-editing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [editorial](../categories/editorial.md)

A strategic engine to transform raw photographic assets into structured editorial roadmaps.

## Description
This MCP server provides a suite of specialized tools for professional photo editors and curators. It automates the transition from raw assets to a finished series by applying selection logic, sequencing rules, and rights compliance. Use `analyze_selection_integrity` to validate candidates against creative goals, `generate_editing_decisions` to categorize images into retain, revise, or exclude, and `construct_sequence_brief` to build narrative flow. The engine ensures that every series adheres to legal constraints via `evaluate_rights_and_compliance` before finalizing the roadmap with `compile_final_plan`.


## Available Tools (5)
- **analyze_selection_integrity**: Validates if candidate images satisfy selection criteria and project statement
- **compile_final_plan**: Aggregates all decisions into a single, actionable editorial document
- **construct_sequence_brief**: Determines the optimal order of images to create a coherent narrative flow
- **evaluate_rights_and_compliance**: Cross-references selected images against legal rights and display format constraints
- **generate_editing_decisions**: Produces the core Retain-Revise-Exclude list for the series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photography Series Editing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these images for a landscape series focused on minimalism."

**🤖 AI Agent:**
> The selection audit confirms that 5 images meet the minimalist criteria, while 2 images were excluded for excessive visual clutter.

---

**👤 You:**
> "Help me decide which images to keep or fix for my portrait project."

**🤖 AI Agent:**
> Based on your criteria, 10 images are marked for retention, 3 require color grading revision, and 2 are excluded due to technical flaws.

---

**👤 You:**
> "Create a sequence for my urban photography series."

**🤖 AI Agent:**
> The sequence starts with a wide establishing shot of the city, followed by three medium shots, and concludes with a tight detail shot of a street sign.


## ❓ FAQ

**Q: How does the tool handle image selection?**
The `analyze_selection_integrity` tool compares your candidate images against your specific project statement and selection criteria to ensure creative alignment.

**Q: Can I ensure my series is legally compliant?**
Yes, by using `evaluate_rights_and_compliance`, the system checks your selected images against your held rights and the intended display format.

**Q: What is the final output of the server?**
The `compile_final_plan` tool aggregates all decisions, sequences, and caption tasks into a single, actionable editorial document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photography-series-editing-plan](https://vinkius.com/en/ai-agent-connect/photography-series-editing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photography Series Editing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photography-series-editing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photography Series Editing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photography-series-editing-plan": {
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
