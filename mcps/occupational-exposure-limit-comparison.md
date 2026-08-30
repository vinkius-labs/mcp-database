# Occupational Exposure Limit Comparison MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/occupational-exposure-limit-comparison)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industrial-hygiene](../categories/industrial-hygiene.md)

Compare chemical concentrations against PEL, TLV, and REL standards.

## Description
This MCP server provides specialized tools for industrial hygiene and safety professionals to assess chemical exposure. It allows for the evaluation of Time-Weighted Average (TWA) compliance using `evaluate_twa_compliance`, assessment of short-term spikes via `evaluate_stel_compliance`, and detailed safety buffer analysis with `calculate_safety_metrics`. Users can also perform multi-standard comparisons using `compare_regulatory_tiers` to check against OSHA PEL, ACGIH TLV, and NIOSH REL simultaneously.


## Available Tools (4)
- **calculate_safety_metrics**: Provides a detailed breakdown of safety buffers and regulatory thresholds
- **compare_regulatory_tiers**: Compares a single measured concentration against multiple regulatory standards simultaneously
- **evaluate_stel_compliance**: Evaluates short-term, high-intensity exposure spikes
- **evaluate_twa_compliance**: Determines if a steady-state exposure over a full shift is within safe limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Occupational Exposure Limit Comparison** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a measured concentration of 0.04 mg/m3 compliant with a PEL of 0.05 mg/m3?"

**🤖 AI Agent:**
> Yes, the concentration is compliant with the PEL.

---

**👤 You:**
> "Check if a 15-minute spike of 5.0 ppm exceeds a STEL of 4.0 ppm."

**🤖 AI Agent:**
> The exposure is non-compliant as it exceeds the STEL.

---

**👤 You:**
> "Compare 0.1 ppm against a PEL of 0.1, a TLV of 0.08, and a REL of 0.12."

**🤖 AI Agent:**
> The status is: PEL is non-compliant, TLV is non-compliant, and REL is compliant.


## ❓ FAQ

**Q: How do I check if my exposure is within legal limits?**
You can use `compare_regulatory_tiers` to check your measured concentration against the OSHA PEL, ACGIH TLV, and NIOSH REL all at once.

**Q: Can I evaluate short-term exposure spikes?**
Yes, use the `evaluate_stel_compliance` tool to determine if a 15-minute concentration exceeds the Short-Term Exposure Limit.

**Q: What is the margin of safety?**
The margin of safety is the ratio between the exposure limit and the measured concentration, which can be calculated using `calculate_safety_metrics`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/occupational-exposure-limit-comparison](https://vinkius.com/ai-agent-connect/occupational-exposure-limit-comparison)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Occupational Exposure Limit Comparison** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `occupational-exposure-limit-comparison` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Occupational Exposure Limit Comparison** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "occupational-exposure-limit-comparison": {
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
