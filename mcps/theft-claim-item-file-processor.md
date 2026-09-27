# Theft Claim Item File Processor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/theft-claim-item-file-processor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Transforms raw theft incident data into structured, evidentiary claim files.

## Description
This MCP server provides a specialized processing engine for insurance claims. It allows AI agents to validate stolen item details using `analyze_item_validity`, cross-reference incident reports with `cross_reference_incident`, verify coverage via `evaluate_policy_coverage`, and compile final evidentiary documents with `generate_claim_file`.


## Available Tools (4)
- **analyze_item_validity**: Determines if the reported stolen item is a valid candidate for a claim based on its description and ownership status
- **cross_reference_incident**: Validates the stolen item details against the official incident report to ensure the claim matches the reported crime
- **evaluate_policy_coverage**: Checks if the stolen item falls under the specific coverage permitted by the user's insurance policy
- **generate_claim_file**: Compiles all analyzed data into a final, structured item file, identifying missing evidence and the necessary steps for submission


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Theft Claim Item File Processor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if this stolen laptop is covered under my policy?"

**🤖 AI Agent:**
> The laptop is covered under your current policy with a coverage limit of $2,500.

---

**👤 You:**
> "Does the incident report match the stolen item description?"

**🤖 AI Agent:**
> Yes, the item description and the incident time and location align with the official report.

---

**👤 You:**
> "Generate a claim file for the reported theft."

**🤖 AI Agent:**
> The claim file has been generated. Status: Pending Evidence. You need to provide a valid serial number for the item.


## ❓ FAQ

**Q: What can this MCP server do?**
It processes theft incident data to create structured claim files, identifying evidence gaps and required submission steps.

**Q: How does it handle policy verification?**
It uses the `evaluate_policy_coverage` tool to check if an item falls under the specific coverage permitted by a user's insurance policy.

**Q: Can it identify missing information?**
Yes, the `generate_claim_file` tool specifically identifies evidence gaps and provides a prioritized submission order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/theft-claim-item-file-processor](https://vinkius.com/en/ai-agent-connect/theft-claim-item-file-processor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Theft Claim Item File Processor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `theft-claim-item-file-processor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Theft Claim Item File Processor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "theft-claim-item-file-processor": {
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
