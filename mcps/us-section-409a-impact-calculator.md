# US Section 409A Impact Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-section-409a-impact-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate legal strike price floors, tax penalties for non-compliant grants, and exercise window rules.

## Description
This MCP server provides essential tools for managing US stock option compliance under Section 409A. It allows AI agents to determine the legal minimum strike price using `calculate_minimum_strike`, estimate financial liabilities with `estimate_tax_penalty`, and understand regulatory windows via `lookup_exercise_rules`. For a complete audit, use `analyze_grant_compliance` to evaluate proposed grants against FMV and option types (ISO/NSO).


## Available Tools (4)
- **lookup_exercise_rules**: Provides regulatory window and tax implications for exercising options
- **analyze_grant_compliance**: A comprehensive audit tool for evaluating a proposed grant scenario
- **calculate_minimum_strike**: Determines the lowest legally permissible strike price
- **estimate_tax_penalty**: Calculates the estimated financial burden if options are granted below FMV


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Section 409A Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum strike price if my current FMV is $15.50?"

**🤖 AI Agent:**
> Based on a current FMV of $15.50, the `calculate_minimum_strike` tool indicates that your minimum legal strike price is $15.50.

---

**👤 You:**
> "Calculate the penalty for a grant with a $12.00 strike price when FMV is $15.00."

**🤖 AI Agent:**
> Using `estimate_tax_penalty`, the taxable spread is $3.00, which triggers a 20% penalty plus applicable interest.

---

**👤 You:**
> "Check if a grant with a $14.00 strike price is compliant for an ISO at $15.00 FMV."

**🤖 AI Agent:**
> The `analyze_grant_compliance` tool identifies this grant as 'Non-Compliant' because the strike price is below the current FMV of $15.00.


## ❓ FAQ

**Q: How can I find the minimum strike price for a new grant?**
Use the `calculate_minimum_strike` tool by providing the current Fair Market Value (FMV) and the valuation date.

**Q: What happens if I grant options below the FMV?**
Granting below FMV triggers a 20% federal penalty tax plus interest. You can use `estimate_tax_penalty` to calculate the projected financial impact.

**Q: Does this tool cover ISO and NSO differences?**
Yes. The `lookup_exercise_rules` tool provides specific exercise windows and tax summaries for both ISO and NSO types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-section-409a-impact-calculator](https://vinkius.com/mcp/us-section-409a-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Section 409A Impact Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-section-409a-impact-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Section 409A Impact Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-section-409a-impact-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
