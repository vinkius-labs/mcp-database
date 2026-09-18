# Training Load Ratio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/training-load-ratio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate Acute:Chronic Workload Ratio (ACWR) to assess injury risk and optimize training.

## Description
This MCP server provides specialized tools for sports scientists and coaches to monitor athlete training loads. By calculating the Acute:Chronic Workload Ratio (ACWR), users can identify if an athlete is under-trained, in the safe zone, or over-trained. The server includes tools like `calculate_acwr` for core ratio calculations, `get_load_recommendations` for physiological adjustments, `validate_training_readiness` for qualitative assessments, and `simulate_load_progression` to predict future risk based on planned workloads.


## Available Tools (4)
- **calculate_acwr**: Calculates the primary ACWR value and determines the risk assessment
- **get_load_recommendations**: Provides specific physiological training adjustments based on a current ACWR
- **simulate_load_progression**: Predicts the future ACWR if a specific planned workload is added
- **validate_training_readiness**: Aggregates load data to provide a qualitative readiness assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Load Ratio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ACWR for an athlete with a weekly load of 50 and a 4-week average of 40 using rolling average."

**🤖 AI Agent:**
> The calculated ACWR is 1.25, which falls within the Safe zone.

---

**👤 You:**
> "What are the training recommendations for an ACWR of 1.6?"

**🤖 AI Agent:**
> The recommendation is to Reduce load to prevent injury, focusing on recovery.

---

**👤 You:**
> "Is an athlete with an acute load of 30 and chronic load of 45 ready for training?"

**🤖 AI Agent:**
> The athlete is currently Under-trained with a risk level of Low.


## ❓ FAQ

**Q: What is the purpose of the ACWR calculation?**
The ACWR compares recent training load (acute) to a long-term baseline (chronic) to help prevent injuries caused by sudden spikes in workload.

**Q: How do I use the `calculate_acwr` tool?**
Provide the current week's load, the 4-week average load, and choose between 'rolling_average' or 'exponential_weighting' as the calculation method.

**Q: Can I predict future injury risk?**
Yes, you can use `simulate_load_progression` to see how a planned workload for next week will impact the athlete's ACWR and risk category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/training-load-ratio](https://vinkius.com/en/ai-agent-connect/training-load-ratio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Load Ratio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-load-ratio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Load Ratio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-load-ratio": {
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
