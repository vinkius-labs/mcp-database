# Gas Injection Miscibility Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-injection-miscibility-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates Minimum Miscibility Pressure (MMP) and analyzes EOR gas injection mechanisms.

## Description
This MCP server provides specialized tools for Enhanced Oil Recovery (EOR) analysis. It allows AI agents to calculate the Minimum Miscibility Pressure (MMP) using `calculate_mmp_correlation`, identify whether a system follows a vaporizing or condensing drive via `analyze_miscibility_mechanism`, quantify how impurities like CO2 or N2 shift pressure requirements with `assess_impurity_impact`, and design hydrocarbon enrichment plans using `evaluate_enrichment_strategy`.


## Available Tools (4)
- **analyze_miscibility_mechanism**: Identify the miscibility mechanism (Vaporizing or Condensing drive)
- **assess_impurity_impact**: Quantify the impact of impurities on the MMP
- **calculate_mmp_correlation**: Estimate Minimum Miscibility Pressure (MMP) using empirical correlations
- **evaluate_enrichment_strategy**: Determine the hydrocarbon enrichment needed to reach a target MMP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Injection Miscibility Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the MMP for a reservoir at 350K using the Alston correlation with a specific oil and gas composition."

**🤖 AI Agent:**
> The calculated Minimum Miscibility Pressure (MMP) using the Alston correlation is 3250 psi, indicating a vaporizing drive mechanism.

---

**👤 You:**
> "What is the impact of adding 5% Nitrogen to my injection gas?"

**🤖 AI Agent:**
> The addition of 5% Nitrogen increases the required MMP by 450 psi, which is categorized as a high impact severity.

---

**👤 You:**
> "Determine if the current pressure of 2800 psi is sufficient for miscibility."

**🤖 AI Agent:**
> At 2800 psi, the system is not miscible as the required MMP is 3100 psi.


## ❓ FAQ

**Q: What is the difference between the correlation types?**
The `calculate_mmp_correlation` tool supports Alston, Glasø, and Yuan models, which use different mathematical approaches to estimate pressure based on fluid properties.

**Q: How does CO2 affect the MMP?**
Using `assess_impurity_impact`, you can see that CO2 typically decreases the required MMP, making it easier to achieve miscibility.

**Q: Can I plan gas enrichment?**
Yes, the `evaluate_enrichment_strategy` tool identifies the specific hydrocarbons needed to lower the MMP to your target level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-injection-miscibility-engine](https://vinkius.com/en/ai-agent-connect/gas-injection-miscibility-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Injection Miscibility Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-injection-miscibility-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Injection Miscibility Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-injection-miscibility-engine": {
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
