# Target Rep Divider MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/target-rep-divider)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Split total repetition targets into equal sets and identify remaining reps.

## Description
The `target-rep-divider` MCP server helps athletes and coaches organize workout volume. Using tools like `generate_repetition_instruction`, you can transform a large total rep goal into a clear, actionable plan of complete sets and a final residual set. It also provides raw data via `calculate_set_breakdown` and ensures your parameters are valid with `validate_repetition_parameters`.


## Available Tools (3)
- **generate_repetition_instruction**: "

Generates a human-readable repetition instruction
- **calculate_set_breakdown**: Calculates the numerical breakdown of sets and remaining reps
- **validate_repetition_parameters**: Validates repetition parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Target Rep Divider** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to do 50 total reps in sets of 12. How should I structure this?"

**🤖 AI Agent:**
> Do 4 sets of 12, and 1 final set of 2 remaining reps.

---

**👤 You:**
> "Calculate the breakdown for 100 reps with 15 reps per set."

**🤖 AI Agent:**
> Do 6 sets of 15, and 1 final set of 10 remaining reps.

---

**👤 You:**
> "Give me instructions for 30 reps in sets of 10."

**🤖 AI Agent:**
> Do 3 sets of 10, and 1 final set of 0 remaining reps.


## ❓ FAQ

**Q: How does the tool calculate sets?**
It uses `calculate_set_breakdown` to divide total reps by reps per set, identifying full sets and any remaining reps.

**Q: Can I use this for hypertrophy training?**
Yes, you can use it to plan high-volume sessions by providing your target repetition count and desired set size.

**Q: What happens if there are leftover reps?**
The `generate_repetition_instruction` tool will explicitly mention the final set containing the remaining repetitions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/target-rep-divider](https://vinkius.com/mcp/target-rep-divider)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Target Rep Divider** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `target-rep-divider` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Target Rep Divider** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "target-rep-divider": {
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
