# Defect Evidence Record MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/defect-evidence-record)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize technical defect evidence and identify evidentiary gaps for warranty claims.

## Description
This MCP server provides tools to automate the assembly of technical defect evidence. It allows AI agents to use `analyze_defect_completeness` to verify if observations meet requirements, `verify_warranty_compliance` to check usage history against warranty rules, `generate_evidence_record` to create structured reports, and `search_evidence_gaps` to pinpoint missing proof. It bridges the gap between raw defect observations and successful warranty claims.


## Available Tools (4)
- **analyze_defect_completeness**: Determines if a single defect observation has enough supporting data to satisfy basic warranty verification
- **generate_evidence_record**: Aggregates observations, usage, and warranty status into a single, organized report
- **search_evidence_gaps**: Identifies specific missing links between a defect observation and its required proof
- **verify_warranty_compliance**: Checks if the product's usage history aligns with the constraints of the warranty


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Defect Evidence Record** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the defect observation 'DEF-123' is complete."

**🤖 AI Agent:**
> The observation 'DEF-123' is incomplete. It is missing a high-resolution photo as required by the warranty rules.

---

**👤 You:**
> "Generate a full evidence record for all current observations."

**🤖 AI Agent:**
> The evidence record has been generated. Status: Incomplete. Summary: Three defects were noted, but two lack sufficient temporal evidence.

---

**👤 You:**
> "Is the usage history compliant with the standard warranty?"

**🤖 AI Agent:**
> No, the usage history is not compliant. The product was used for 'Commercial' purposes, which is not allowed under the Standard Tier warranty.


## ❓ FAQ

**Q: How does this server help with warranty claims?**
It uses `generate_evidence_record` to aggregate observations and usage history, identifying exactly what is missing to satisfy warranty requirements.

**Q: Can I check if my product usage violates the warranty?**
Yes, the `verify_warranty_compliance` tool checks if the recorded usage history aligns with the constraints defined in the warranty rules.

**Q: What happens if my evidence is incomplete?**
You can use `search_evidence_gaps` to find out which specific types of proof, such as high-resolution photos or timestamps, are still required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/defect-evidence-record](https://vinkius.com/en/ai-agent-connect/defect-evidence-record)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Defect Evidence Record** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `defect-evidence-record` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Defect Evidence Record** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "defect-evidence-record": {
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
