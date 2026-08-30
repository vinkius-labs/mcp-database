# Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Precise volume calculations for single-step and serial dilutions.

## Description
This MCP server provides laboratory professionals with precise tools for solution chemistry. Use `calculate_single_dilution` to find exact stock and diluent volumes for one-step processes. For large dilution factors, `calculate_serial_dilution_plan` generates a multi-step sequence to maintain accuracy. You can also use `validate_mixing_ratio` to verify if your parts-based ratios are mathematically consistent with target concentrations.


## Available Tools (4)
- **calculate_serial_dilution_plan**: Generates a multi-step dilution sequence when a single step is impractical
- **calculate_single_dilution**: Calculates the specific volumes needed for a one-step dilution
- **get_dilution_factor_info**: Provides descriptive metadata about a specific dilution factor
- **validate_mixing_ratio**: Checks if a specific ratio of stock to diluent is mathematically consistent with the target concentrations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 10M stock solution. I need 500ml of a 0.1M solution. How much stock and diluent do I need?"

**🤖 AI Agent:**
> You need 5ml of the 10M stock solution and 495ml of diluent to reach a total volume of 500ml.

---

**👤 You:**
> "Plan a serial dilution for a 1000-fold dilution starting from 1M, with a max dilution factor of 10 per step."

**🤖 AI Agent:**
> The plan requires 3 steps: Step 1 (1:10) results in 0.1M, Step 2 (1:10) results in 0.01M, and Step 3 (1:10) results in 0.001M.

---

**👤 You:**
> "Is a 1:5 ratio of stock to diluent correct for a 1M to 0.2M dilution?"

**🤖 AI Agent:**
> Yes, a 1:5 ratio (1 part stock to 4 parts diluent) results in a 1:5 dilution factor, which is correct for 1M to 0.2M.


## ❓ FAQ

**Q: How do I calculate a single dilution step?**
Use the `calculate_single_dilution` tool by providing the initial concentration, the desired final concentration, and the total final volume.

**Q: When should I use a serial dilution plan?**
Use `calculate_serial_dilution_plan` when the required dilution factor is too large to achieve accurately in a single step.

**Q: Can I verify my mixing ratios?**
Yes, the `validate_mixing_ratio` tool checks if your stock and diluent parts match the required dilution factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dilution-calculator](https://vinkius.com/ai-agent-connect/dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dilution-calculator": {
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
