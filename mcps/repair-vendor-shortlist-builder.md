# Repair Vendor Shortlist Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-vendor-shortlist-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [procurement](../categories/procurement.md)

An intelligent decision-support engine that transforms raw vendor data and custom weighted rubrics into a ranked, auditable shortlist.

## Description
This MCP server provides a suite of tools to automate vendor selection and procurement workflows. It allows users to input raw vendor profiles, apply strict disqualification criteria, and use a weighted rubric to rank candidates. Key capabilities include generating a prioritized shortlist via `get_ranked_shortlist`, creating targeted investigative questions with `generate_due_diligence_plan`, designing communication timelines with `get_outreach_workflow`, and producing transparent scoring logs with `get_audit_table`.


## Available Tools (4)
- **generate_due_diligence_plan**: 
- **get_audit_table**: 
- **get_outreach_workflow**: 
- **get_ranked_shortlist**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Vendor Shortlist Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these vendors: Vendor A (Score 8, Weight 1), Vendor B (Score 5, Weight 1). Disqualify anyone without insurance."

**🤖 AI Agent:**
> Vendor A: 8.0, Vendor B: 5.0.

---

**👤 You:**
> "Generate due diligence questions for the top vendor, focusing on insurance coverage."

**🤖 AI Agent:**
> 1. Can you provide proof of your current liability insurance limits? 2. Does your coverage extend to emergency repair scenarios?

---

**👤 You:**
> "Create an outreach plan for an Emergency Repair project for Vendor A."

**🤖 AI Agent:**
> Step 1: Immediate contact via phone. Step 2: Send formal Request for Quote. Step 3: Confirm availability for immediate dispatch.


## ❓ FAQ

**Q: How does the scoring logic work?**
The engine calculates a final score by multiplying each criterion's value by its assigned weight in the rubric. You can use `get_audit_table` to see the exact mathematical breakdown for every vendor.

**Q: Can I disqualify vendors automatically?**
Yes. By providing disqualification criteria to the `get_ranked_shortlist` tool, any vendor failing a hard constraint is immediately removed from the results.

**Q: What happens after I select a vendor?**
You can use `get_outreach_workflow` to generate a structured communication timeline, moving from initial contact to final engagement based on your project type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-vendor-shortlist-builder](https://vinkius.com/en/ai-agent-connect/repair-vendor-shortlist-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Vendor Shortlist Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-vendor-shortlist-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Vendor Shortlist Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-vendor-shortlist-builder": {
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
