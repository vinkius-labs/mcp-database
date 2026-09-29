# Repair Service Agreement Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-service-agreement-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal-tech](../categories/legal-tech.md)

Audit service agreements to identify missing contractual components and generate actionable checklists.

## Description
This MCP server provides a suite of diagnostic tools to audit service agreements. It identifies missing mandatory pillars such as Quote, Responsibilities, Warranty, and Schedule. Users can use `analyze_agreement_completeness` to find gaps, `generate_clarification_questions` to resolve ambiguities, `map_missing_details` to categorize omissions into Financial, Legal, Operational, or Temporal buckets, and `create_acceptance_checklist` to verify the agreement against original user requirements.


## Available Tools (4)
- **create_acceptance_checklist**: 
- **generate_clarification_questions**: 
- **map_missing_details**: 
- **analyze_agreement_completeness**: Identifies which standard agreement pillars are missing from the provided input


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Service Agreement Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have an agreement with only 'Quote' and 'Responsibilities'. What is missing?"

**🤖 AI Agent:**
> The mandatory missing pillars are Warranty and Schedule.

---

**👤 You:**
> "The agreement is missing the warranty details. What should I ask the provider?"

**🤖 AI Agent:**
> You should ask: 'What is the specific duration of the warranty and what are the exact coverage limits?'

---

**👤 You:**
> "My requirement is that the work must be finished by next Tuesday. The contract says 'completion in 5 days'. Is this okay?"

**🤖 AI Agent:**
> No, the contract does not guarantee completion by next Tuesday.


## ❓ FAQ

**Q: How do I know if my agreement is complete?**
You can use the `analyze_agreement_completeness` tool by providing the list of fields currently in your document to receive a completeness score and a list of missing pillars.

**Q: Can I organize missing information by category?**
Yes, the `map_missing_details` tool categorizes all identified omissions into Financial, Legal, Operational, or Temporal domains.

**Q: How can I verify the agreement meets my specific needs?**
Use the `create_acceptance_checklist` tool. It compares your original user requirements against the extracted contract terms to generate a Yes/No verification list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-service-agreement-auditor](https://vinkius.com/en/ai-agent-connect/repair-service-agreement-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Service Agreement Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-service-agreement-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Service Agreement Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-service-agreement-auditor": {
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
