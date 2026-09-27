# Landlord Repair Request Package MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/landlord-repair-request-package)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured, legally-defensible repair request packages from tenancy evidence.

## Description
This MCP server transforms disorganized tenant communications into a professional, ready-to-file repair request package. It uses a strict Chronological Evidence Rule to organize facts and ensures all claims are backed by an attachment index. Users can use `generate_repair_request` to create formal notices, `create_attachment_index` to link photos and messages to specific claims, `calculate_followup_plan` to track legal notice deadlines, and `compile_escalation_record` to produce objective summaries for mediators or legal authorities.


## Available Tools (4)
- **calculate_followup_plan**: Generates a timeline of future actions to ensure the tenant stays within legal notice windows
- **compile_escalation_record**: Produces a high-level, objective summary for third-party mediators or legal authorities
- **create_attachment_index**: Maps provided evidence to the facts in the repair request
- **generate_repair_request**: Creates the formal, written request for repairs sent to the landlord


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Landlord Repair Request Package** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a major leak in my kitchen that started two days ago. I've sent one message to my landlord but haven't heard back. Help me prepare a request."

**🤖 AI Agent:**
> I have generated your formal repair request citing the relevant lease clauses. I have also created an attachment index for your photos of the leak and calculated that your next follow-up should occur in 5 days based on the 'Major' issue severity.

---

**👤 You:**
> "Create an attachment index for my repair claim using these photos: photo_01.jpg, photo_02.jpg and the claim 'The ceiling is water damaged'."

**🤖 AI Agent:**
> The attachment index is complete. Claim 'The ceiling is water damaged' is now linked to photo_01.jpg and photo_02.jpg.

---

**👤 You:**
> "Generate an escalation record for my ongoing dispute regarding the broken heater."

**🤖 AI Agent:**
> The escalation record has been compiled. It contains a neutral summary of the timeline, a full evidence manifest, and confirms that the legal escalation window is now open.


## ❓ FAQ

**Q: How does the tool ensure the repair request is legally defensible?**
The system applies a Chronological Evidence Rule and requires an attachment index to ensure every factual claim is directly linked to specific evidence like photos or messages.

**Q: Can I use this to prepare for a tribunal or court hearing?**
Yes. By using `compile_escalation_record`, you can generate a neutral, third-person summary designed specifically for third-party mediators or legal authorities.

**Q: How are notice deadlines handled?**
The `calculate_followup_plan` tool uses your provided notice deadlines and issue severity to calculate exactly when you should next contact the landlord and when the escalation window opens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/landlord-repair-request-package](https://vinkius.com/en/ai-agent-connect/landlord-repair-request-package)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Landlord Repair Request Package** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `landlord-repair-request-package` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Landlord Repair Request Package** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "landlord-repair-request-package": {
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
