# Claim Reopen Request Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/claim-reopen-request-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Generates professional, factual insurance claim reopening requests based on new evidence and policy context.

## Description
This MCP server provides a suite of tools to automate the creation of formal insurance claim reopening requests. By providing a prior decision, new evidence, and policy references, users can use `generate_reopen_request` to produce a structured document that links new findings to specific policy clauses. The server also includes `validate_timeline_integrity` to ensure claim histories are chronologically sound, `match_evidence_to_policy` to identify relevant coverage triggers, and `format_attachment_list` to organize evidence into a professional attachment summary.


## Available Tools (4)
- **generate_reopen_request**: Compiles all provided data points into a structured, professional, and factual formal request document
- **match_evidence_to_policy**: Identifies which policy clauses are most relevant to the new evidence provided
- **validate_timeline_integrity**: Ensures the provided claim history is logical and chronologically sound
- **format_attachment_list**: Organizes the newRecords into a clean, numbered list of formal attachments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claim Reopen Request Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a reopen request for claim #12345. The original decision denied coverage for water damage. However, I have a new certified engineering report showing the damage was caused by a pipe burst, not flooding. Policy section 4.2 covers pipe bursts."

**🤖 AI Agent:**
> Formal Reopen Request: Claim #12345. Based on the new certified engineering report (Attachment 1), the previous decision denying coverage for water damage is contested. Under Policy Section 4.2, pipe bursts are covered, and the new evidence confirms the cause was a pipe burst rather than flooding.

---

**👤 You:**
> "I need to check if my claim timeline is correct: Jan 1st - Loss reported, Jan 5th - Investigation started, Jan 3rd - Initial decision."

**🤖 AI Agent:**
> The timeline is invalid. The event 'Initial decision' on Jan 3rd occurs before 'Investigation started' on Jan 5th, violating chronological order.

---

**👤 You:**
> "Format these new records into an attachment list: Medical report from Dr. Smith, and a receipt for repairs."

**🤖 AI Agent:**
> Attachment 1: Medical report from Dr. Smith
Attachment 2: Receipt for repairs


## ❓ FAQ

**Q: How do I ensure my claim timeline is valid?**
You can use the `validate_timeline_integrity` tool to check if your claim history is in strictly ascending order and contains no future dates before generating your request.

**Q: Can this tool help me find relevant policy clauses?**
Yes, the `match_evidence_to_policy` tool analyzes the semantic relationship between your new evidence and your policy references to identify which clauses are impacted.

**Q: What is the final output of the generator?**
The `generate_reopen_request` tool produces a structured, professional document ready for submission, including a formatted list of attachments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/claim-reopen-request-generator](https://vinkius.com/en/ai-agent-connect/claim-reopen-request-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claim Reopen Request Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claim-reopen-request-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claim Reopen Request Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claim-reopen-request-generator": {
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
