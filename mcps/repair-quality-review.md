# Repair Quality Review MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-quality-review)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Automated quality assurance that compares repair scopes against completion results.

## Description
This MCP server provides an automated quality assurance engine for repair services. It synthesizes data from repair scopes, completion reports, functional tests, and visual evidence to generate actionable pickup checklists and identify unresolved issues. Use `analyze_repair_completeness` to verify deliverables, `verify_functional_integrity` to check performance tolerances, `evaluate_visual_compliance` to confirm physical work via photos, and `generate_quality_summary` to produce the final customer report.


## Available Tools (4)
- **analyze_repair_completeness**: Determines if the work documented in the completion report satisfies the requirements of the original repair scope
- **evaluate_visual_compliance**: Uses visual evidence to verify that the physical work matches the reported work
- **generate_quality_summary**: Aggregates all findings into a final output for the customer
- **verify_functional_integrity**: Compares the results of post-repair function checks against the required performance standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Quality Review** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the repair was completed according to the scope."

**🤖 AI Agent:**
> The repair is complete. All requested items in the scope were found in the completion report, and all functional tests passed.

---

**👤 You:**
> "Generate a quality summary for the customer."

**🤖 AI Agent:**
> Pickup Checklist: 1. Verify new brake pads installation. 2. Confirm fluid levels. Follow-up Issues: 1. Visual: Minor scratch on left fender.

---

**👤 You:**
> "Verify if the visual evidence matches the reported work."

**🤖 AI Agent:**
> The visual evidence confirms the installation of the new component as reported.


## ❓ FAQ

**Q: What does this server do?**
It automates the comparison between what was planned in a repair scope and what was actually performed, providing a final checklist for customers.

**Q: How can I use the visual verification tool?**
You can use `evaluate_visual_compliance` by providing a photo set ID and the specific work item ID to verify if the physical repair matches the report.

**Q: Does it support functional testing?**
Yes, `verify_functional_integrity` allows you to check if post-repair measurements fall within your required performance thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-quality-review](https://vinkius.com/en/ai-agent-connect/repair-quality-review)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Quality Review** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-quality-review` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Quality Review** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-quality-review": {
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
