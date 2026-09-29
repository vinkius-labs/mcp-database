# Warranty Exclusion Question Set MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/warranty-exclusion-question-set)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal-tech](../categories/legal-tech.md)

Generates neutral, fact-based inquiries to bridge defects and warranty exclusions.

## Description
This MCP server provides a specialized diagnostic framework for service providers. It transforms raw technical observations into neutral, non-leading questions. By using tools like `generate_fact_queries` and `align_with_exclusions`, it identifies technical overlaps between product defects and specific warranty exclusion clauses without performing subjective legal judgments. It helps gather the necessary facts to allow human experts to make informed coverage decisions.


## Available Tools (4)
- **align_with_exclusions**: Align defect facts with exclusion wording
- **cross_reference_history**: Identify discrepancies between current defect and service history
- **generate_fact_queries**: Transform raw defect observations into neutral questions
- **synthesize_final_question_set**: Consolidate findings into a final set of questions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Warranty Exclusion Question Set** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a defect: 'corroded wiring in the main power unit'. The evidence is 'photographic'. Generate questions."

**🤖 AI Agent:**
> 1. What specific environmental conditions were present near the power unit? 2. At what point in the device's lifecycle was the corrosion first observed? 3. Are there signs of moisture ingress in the surrounding housing?

---

**👤 You:**
> "The exclusion clause says 'damage caused by unauthorized modification'. The defect is 'cracked housing'. Use `align_with_exclusions` to find gaps."

**🤖 AI Agent:**
> Matching parameters: None. Unanswered fact gaps: Evidence of whether the housing was opened or tampered with by non-authorized personnel.

---

**👤 You:**
> "The current defect is 'software timeout'. The service history shows 'firmware update performed 2 days ago'. Use `cross_reference_history`."

**🤖 AI Agent:**
> The current defect is in the same subsystem as a service event from two days ago.


## ❓ FAQ

**Q: Does this tool decide if a warranty claim is valid?**
No. The tool is designed for interpretation avoidance. It uses `align_with_exclusions` to find technical overlaps, but it does not make legal or coverage judgments. It provides the facts needed for a human to make that decision.

**Q: How does it ensure questions are neutral?**
The `generate_fact_queries` tool is specifically programmed to strip accusatory or interpretive language, focusing strictly on 'what', 'when', and 'how' regarding the physical state of the item.

**Q: Can I use this with Claude Desktop?**
Yes. You can connect this MCP to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/warranty-exclusion-question-set](https://vinkius.com/en/ai-agent-connect/warranty-exclusion-question-set)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Warranty Exclusion Question Set** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `warranty-exclusion-question-set` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Warranty Exclusion Question Set** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "warranty-exclusion-question-set": {
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
