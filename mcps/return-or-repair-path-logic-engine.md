# Return or Repair Path Logic Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/return-or-repair-path-logic-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [decision-support](../categories/decision-support.md)

Generates step-by-step resolution roadmaps for consumer product claims.

## Description
This MCP server provides a logic engine to analyze consumer purchase data and product warranty terms. It uses `analyze_eligibility` to check return and warranty windows, `evaluate_defect_validity` to assess proof strength, and `check_deadline_compliance` to verify reporting timelines. Finally, `generate_resolution_path` synthesizes these inputs into a clear, actionable roadmap for achieving a refund, repair, or replacement.


## Available Tools (4)
- **analyze_eligibility**: Determines if a consumer is still within the legal or contractual windows required to seek a remedy
- **check_deadline_compliance**: Verifies if the consumer has missed any critical intermediate deadlines
- **evaluate_defect_validity**: Assesses whether the provided evidence is sufficient to trigger a remedy
- **generate_resolution_path**: Synthesizes prior analysis to produce a step-by-step instructional roadmap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Return or Repair Path Logic Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought a laptop 10 days ago, the return window is 30 days, the warranty is 365 days, it is currently 2024-01-15, I have a photo of a broken screen (strength 90/100), the threshold is 70, and I discovered the defect today. I want a refund."

**🤖 AI Agent:**
> 1. Return to Vendor. 2. Present photographic evidence of the broken screen. 3. Complete the refund process at the point of purchase.

---

**👤 You:**
> "My phone warranty is valid for 730 days. I bought it 400 days ago. The warranty is still active. I have a technical report (strength 85/100) and the threshold is 80. I discovered the issue 2 days ago and am reporting it today. The deadline is 5 days. I want a repair."

**🤖 AI Agent:**
> 1. Manufacturer Service Request. 2. Submit the technical report to the service center. 3. Await repair confirmation.

---

**👤 You:**
> "I bought a camera 400 days ago. The return window was 30 days and the warranty was 365 days. I want a refund."

**🤖 AI Agent:**
> Claim Denied. The product is outside both the return window and the warranty period.


## ❓ FAQ

**Q: How does the engine determine if I can return my product?**
The engine uses the `analyze_eligibility` tool to compare your purchase date against the allowed return window days to see if you are still eligible for a refund.

**Q: What happens if my evidence is not strong enough?**
If `evaluate_defect_validity` determines the evidence strength is below the required threshold, the generated resolution path will include steps for providing additional proof.

**Q: Can this tool help with warranty claims?**
Yes. By using `analyze_eligibility` and `generate_resolution_path`, the engine can identify if a product is within its warranty period and provide a path for manufacturer service requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/return-or-repair-path-logic-engine](https://vinkius.com/en/ai-agent-connect/return-or-repair-path-logic-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Return or Repair Path Logic Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `return-or-repair-path-logic-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Return or Repair Path Logic Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "return-or-repair-path-logic-engine": {
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
