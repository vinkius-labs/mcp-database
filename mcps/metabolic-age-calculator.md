# Metabolic Age Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/metabolic-age-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Determine your metabolic age and efficiency compared to your chronological age.

## Description
This MCP server provides tools to calculate metabolic age by comparing Basal Metabolic Rate (BMR) against demographic benchmarks. Use `get_metabolic_profile` to find your metabolic age, age difference, and percentile ranking. You can also use `get_improvement_plan` to receive actionable lifestyle recommendations based on your results, or `validate_bmr_range` to ensure your BMR input is physiologically plausible.


## Available Tools (4)
- **get_demographic_benchmarks**: Retrieves statistical averages for BMR used for comparison logic
- **get_improvement_plan**: Provides actionable lifestyle recommendations based on the metabolic gap
- **get_metabolic_profile**: Calculates core metabolic age metrics based on user physical data
- **validate_bmr_range**: Verifies if a provided BMR is within physiologically plausible limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metabolic Age Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my metabolic profile. I am a 35-year-old male, 180cm tall, weighing 85kg, with a BMR of 1850 calories."

**🤖 AI Agent:**
> Your metabolic age is 32, which is 3 years younger than your chronological age. You are in the 65th percentile for metabolic efficiency. Your assessment status is 'Excellent'.

---

**👤 You:**
> "What is a good improvement plan for a 45-year-old female with a metabolic age of 50?"

**🤖 AI Agent:**
> To improve your metabolic efficiency, your primary focus should be Muscle Mass Accretion. We recommend increasing protein intake and starting a regular resistance training program. Your target metabolic age is 42.

---

**👤 You:**
> "Is a BMR of 1200 calories realistic for a 25-year-old male?"

**🤖 AI Agent:**
> The BMR value of 1200 is within the plausible range for your demographic, though it is on the lower end of the expected spectrum.


## ❓ FAQ

**Q: What is metabolic age?**
Metabolic age is a metric that represents how your metabolism is performing relative to your actual age. A lower metabolic age suggests a more efficient metabolism.

**Q: How accurate is the BMR validation?**
The `validate_bmr_range` tool uses demographic-specific statistical data to check if your provided BMR is within physiologically plausible limits for your age and gender.

**Q: Can I get a plan to improve my metabolic age?**
Yes, after calculating your profile, you can use `get_improvement_plan` to receive specific lifestyle recommendations like resistance training or dietary adjustments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/metabolic-age-calculator](https://vinkius.com/en/ai-agent-connect/metabolic-age-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metabolic Age Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metabolic-age-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metabolic Age Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metabolic-age-calculator": {
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
