# Well Stimulation Evaluation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-stimulation-evaluation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Assess the effectiveness of well stimulation treatments using skin factor and productivity metrics.

## Description
This MCP server provides analytical tools to evaluate the performance impact of well stimulation treatments. By comparing pre- and post-treatment reservoir metrics, users can determine the success of operations like acidizing or hydraulic fracturing. Key capabilities include using `analyze_skin_impact` to measure damage removal, `calculate_productivity_gain` to determine fluid production increases, and `evaluate_treatment_efficiency` to assess technical effectiveness based on cost and damage type. The `summarize_well_performance` tool provides a final performance status snapshot.


## Available Tools (4)
- **analyze_skin_impact**: Calculates how effectively the treatment removed near-wellbore damage
- **calculate_productivity_gain**: Determines the relative increase in the well's ability to produce fluids
- **evaluate_treatment_efficiency**: Assesses the technical effectiveness of the specific treatment method used
- **summarize_well_performance**: Provides a comprehensive snapshot of the well's state change


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Stimulation Evaluation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the skin reduction if the pre-treatment skin factor was 5.0 and the post-treatment was 1.0."

**🤖 AI Agent:**
> The skin reduction is 4.0.

---

**👤 You:**
> "What is the productivity improvement ratio if the pre-treatment PI was 1.5 and the post-treatment PI is 3.0?"

**🤖 AI Agent:**
> The productivity improvement ratio is 2.0, representing a 100% increase.

---

**👤 You:**
> "Summarize the performance for a well where pre-treatment data is {'pi': 1.0, 'skin': 4.0} and post-treatment data is {'pi': 2.5, 'skin': 0.5}."

**🤖 AI Agent:**
> The performance status is Highly Successful.


## ❓ FAQ

**Q: How do I know if my stimulation was successful?**
You can use `summarize_well_performance` to get a status rating, or `calculate_productivity_gain` to see the specific increase in the productivity index.

**Q: What is skin reduction?**
Skin reduction is the change in the skin factor resulting from the treatment, calculated via `analyze_skin_impact`.

**Q: Can I evaluate the cost-effectiveness of a treatment?**
Yes, the `evaluate_treatment_efficiency` tool assesses technical effectiveness by weighing skin reduction against the treatment cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-stimulation-evaluation](https://vinkius.com/ai-agent-connect/well-stimulation-evaluation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Stimulation Evaluation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-stimulation-evaluation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Stimulation Evaluation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-stimulation-evaluation": {
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
