# Repair Scope Change Request Assistant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-scope-change-request-assistant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Draft factual scope-change requests and response deadlines for project management.

## Description
This MCP server provides a suite of tools to manage project scope deviations. It allows users to verify if an observed issue constitutes a formal change using `analyze_scope_discrepancy`, assess financial viability with `validate_budget_impact`, and determine critical response dates via `calculate_deadline`. Finally, it synthesizes all findings into a professional document using `generate_scr_draft`.


## Available Tools (4)
- **analyze_scope_discrepancy**: Determine if a newly discovered issue constitutes a change from the original agreement
- **calculate_deadline**: Determine when a decision is needed to maintain project momentum
- **generate_scr_draft**: Synthesize data into a professional, factual request for approval
- **validate_budget_impact**: Check if the proposed change is financially viable within project constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Scope Change Request Assistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I found a broken pipe that wasn't in the original plumbing scope. The repair quote is $500. My budget cap is $2000 and I've already spent $1200. What should I do?"

**🤖 AI Agent:**
> The total projected cost is $1700, which is within your $2000 budget cap. You should proceed with the `generate_scr_draft` tool to formalize the request for approval.

---

**👤 You:**
> "The foundation is cracked, which is a major issue. The quote is $5000. My remaining budget is $2000 and the cap is $5000. Is this a problem?"

**🤖 AI Agent:**
> Yes, this is a critical issue. The total projected cost of $7000 exceeds your $5000 budget cap by $2000.

---

**👤 You:**
> "I need to draft a change request for a new electrical panel. The quote is $1200. The original scope was just wiring. The urgency is high."

**🤖 AI Agent:**
> I will use `analyze_scope_discrepancy` to confirm the change, `calculate_deadline` to set a 24-hour response window, and then `generate_scr_draft` to create the formal document.


## ❓ FAQ

**Q: How do I know if an issue is a scope change?**
You can use the `analyze_scope_discrepancy` tool to compare the original agreement against the newly discovered issue.

**Q: Can this tool help with budget overruns?**
Yes, the `validate_budget_impact` tool calculates if a new quote will exceed your project's budget cap.

**Q: How is the response deadline determined?**
The `calculate_deadline` tool sets deadlines based on urgency: 24 hours for high, 3 days for medium, and 7 days for low urgency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-scope-change-request-assistant](https://vinkius.com/en/ai-agent-connect/repair-scope-change-request-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Scope Change Request Assistant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-scope-change-request-assistant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Scope Change Request Assistant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-scope-change-request-assistant": {
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
