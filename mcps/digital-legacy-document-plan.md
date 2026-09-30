# Digital Legacy Document Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-legacy-document-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synthesize digital assets and contacts into a structured legacy record with completeness checklists and review schedules.

## Description
This MCP server provides a planning engine to manage the transition of digital ownership. It maps technical assets like accounts, devices, and encrypted storage to designated contacts. Use `compile_legacy_plan` to generate a unified view of your digital estate, including a completeness checklist and a proactive review schedule. You can also use `analyze_asset_coverage` to identify critical gaps in your documentation.


## Available Tools (4)
- **analyze_asset_coverage**: Determines if the user has sufficiently documented all critical digital components
- **compile_legacy_plan**: Synthesizes all data into a cohesive summary of the user's legacy readiness
- **generate_review_schedule**: Calculates a timeline of future dates for the user to review and update their plan
- **validate_contact_assignment**: Checks if the designated contacts are appropriate and sufficiently mapped to the assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Legacy Document Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if my digital assets are sufficiently documented?"

**🤖 AI Agent:**
> Your current completeness score is 75%. You have critical gaps in your encrypted storage assets which lack a designated contact.

---

**👤 You:**
> "Generate a review schedule for my legacy plan with a 6-month interval."

**🤖 AI Agent:**
> Your next review is scheduled for June 15, 2024. Subsequent reviews are set for December 15, 2024, and June 15, 2025.

---

**👤 You:**
> "Compile my full legacy plan with my current assets and contacts."

**🤖 AI Agent:**
> Your legacy plan is ready. It includes a completeness checklist showing 4 secured assets and 2 vulnerabilities, along with a review schedule for the next 12 months.


## ❓ FAQ

**Q: How do I know if my digital estate is fully documented?**
You can use the `analyze_asset_coverage` tool to receive a completeness score and identify any critical gaps in your asset documentation.

**Q: Can I schedule regular updates for my plan?**
Yes, the `generate_review_schedule` tool calculates a timeline of future dates based on your preferred review interval.

**Q: What information is required to create a full legacy plan?**
To use `compile_legacy_plan`, you need to provide your accounts, devices, encrypted storage, contacts, and document locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-legacy-document-plan](https://vinkius.com/en/ai-agent-connect/digital-legacy-document-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Legacy Document Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-legacy-document-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Legacy Document Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-legacy-document-plan": {
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
