# Disaster Insurance Records Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/disaster-insurance-records-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize property evidence and insurance details for rapid disaster recovery.

## Description
This MCP server provides tools to manage property evidence and insurance readiness. Use `get_insurance_records_packet` to compile a claim-ready dossier, `calculate_update_cadence` to schedule record reviews, `get_claim_contact_card` for immediate insurer contact during emergencies, and `identify_missing_evidence` to find gaps in your documentation like missing photos or receipts.


## Available Tools (4)
- **calculate_update_cadence**: Determine when the user next needs to review their records
- **get_claim_contact_card**: Provide a highly readable summary of insurer contact information
- **get_insurance_records_packet**: Compile a complete, claim-ready dossier of all assets and policies
- **identify_missing_evidence**: Pinpoint exactly what is missing to make a claim successful


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Disaster Insurance Records Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you show me my insurance records packet for policy POL-123?"

**🤖 AI Agent:**
> Here is your claim-ready dossier for policy POL-123. It includes your verified inventory, evidence manifest, and a readiness score of 85%.

---

**👤 You:**
> "What is the contact information for my current insurance policy?"

**🤖 AI Agent:**
> Your primary contact for this policy is Insurer Corp at 555-0199. Please call them first, then document any damage.

---

**👤 You:**
> "Check if I have any missing evidence for my policy."

**🤖 AI Agent:**
> You have 3 items missing documentation. Specifically, you need to upload a receipt for the high-value electronics and a photo for the living room furniture.


## ❓ FAQ

**Q: How do I know if my records are ready for a claim?**
You can use `get_insurance_records_packet` to check your readiness score, which evaluates if items have both photos and receipts.

**Q: What should I do if I am missing documentation?**
Use `identify_missing_evidence` to generate a prioritized checklist of missing photos, receipts, or redundant storage requirements.

**Q: How often should I update my insurance records?**
The `calculate_update_cadence` tool determines your next review date based on your last audit and the value of your assets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/disaster-insurance-records-plan](https://vinkius.com/en/ai-agent-connect/disaster-insurance-records-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Disaster Insurance Records Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `disaster-insurance-records-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Disaster Insurance Records Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disaster-insurance-records-plan": {
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
