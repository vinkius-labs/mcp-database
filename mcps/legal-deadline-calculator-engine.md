# Legal Deadline Calculator Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legal-deadline-calculator-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compute rigorous procedural deadlines in business days without risking LLM mathematical hallucination.

## Description
In the legal profession, missing a deadline is catastrophic. Language models notoriously fail at date math, completely ignoring weekends and national holidays when asked to add 15 business days. This engine performs exact, local procedural deadline computations. By natively processing ISO dates and explicitly skipping non-business days and user-provided holidays, it ensures your autonomous legal agents never miss a filing date.


## Available Tools
- **calculate_legal_deadline**: Provide optional holidays to skip.

Calculates exact procedural deadlines in business days, skipping weekends and optional holidays


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legal Deadline Calculator Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The client was subpoenaed on 2026-05-15. Add exactly 15 business days to calculate the final deadline."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Calculate the 10-business-day deadline starting from October 10th, 2026, and make sure to skip the national holiday on October 12th."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "I need to file an appeal in 5 business days from December 20th, 2026. Provide the exact date considering December 25th is a holiday."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: Does it automatically know all holidays?**
No, to remain globally deterministic and local, the agent must pass an array of specific holiday dates (e.g., local state holidays) to be skipped during the count.

**Q: Does it count the start date?**
No. In accordance with most civil procedural rules (like the Brazilian CPC), the count begins on the first business day *after* the start date.

**Q: Is this secure for client data?**
Absolutely. The engine executes locally within the Vinkius Edge runtime, meaning no deadline inquiries are sent to external APIs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legal-deadline-calculator-engine](https://vinkius.com/mcp/legal-deadline-calculator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legal Deadline Calculator Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `legal-deadline-calculator-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legal Deadline Calculator Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legal-deadline-calculator-engine": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
