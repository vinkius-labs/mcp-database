# Cancellation Claim Packet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cancellation-claim-packet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Maps travel documents to insurance claim fields to generate structured assembly plans.

## Description
This MCP server acts as an intelligent mapping engine for insurance claims. It analyzes fragmented travel documents--including receipts, booking terms, and communications--to align them with specific policy requirements. Using tools like `map_evidence_to_fields` and `validate_claim_completeness`, it identifies evidence gaps and verifies if a claim is ready for submission. It bridges the gap between raw evidence and structured insurance requirements.


## Available Tools (4)
- **map_evidence_to_fields**: Analyzes all provided documents to determine which insurance claim fields are satisfied and which are missing
- **validate_claim_completeness**: Checks the generated assembly plan against the policy requirements to ensure the claim is submission-ready
- **get_document_metadata_index**: Returns a searchable index of all uploaded documents
- **summarize_evidence_gaps**: Provides a human-readable list of what is missing to help the user collect the necessary documents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cancellation Claim Packet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Map these documents to my insurance claim requirements."

**🤖 AI Agent:**
> I have mapped your receipts and cancellation email to the 'Proof of Loss' and 'Reason for Cancellation' fields. There is currently a gap for 'Proof of Medical Necessity'.

---

**👤 You:**
> "Is my claim ready for submission?"

**🤖 AI Agent:**
> Yes, all mandatory requirements are mapped with high confidence. Your claim is ready.

---

**👤 You:**
> "What is missing from my claim packet?"

**🤖 AI Agent:**
> You are missing the original booking confirmation. Please upload the contract from your airline to satisfy the 'Contractual Terms' requirement.


## ❓ FAQ

**Q: How does the tool identify missing documents?**
The `summarize_evidence_gaps` tool analyzes the assembly plan to find requirements that have no corresponding evidence, providing a list of missing items and suggested actions.

**Q: Can I check if my claim is ready to submit?**
Yes, you can use `validate_claim_completeness` to check your assembly plan against policy requirements to ensure it is submission-ready.

**Q: What kind of documents can I use?**
You can provide financial receipts, contractual booking terms, event-based evidence like doctor notes, and communicative logs like email threads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cancellation-claim-packet](https://vinkius.com/en/ai-agent-connect/cancellation-claim-packet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cancellation Claim Packet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cancellation-claim-packet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cancellation Claim Packet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cancellation-claim-packet": {
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
