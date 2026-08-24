# Accelerator Founder Personality Fit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-founder-personality-fit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Evaluate the alignment between startup founders and accelerator programs using psychological profiling.

## Description
This MCP server provides a diagnostic suite to assess how well a founder or founding team matches an accelerator program. By analyzing psychological traits, cultural synergy, and coaching compatibility, it calculates a holistic fit score. Use `calculate_fit_score` for an aggregate assessment, `analyze_coaching_match` to identify mentorship friction, `evaluate_culture_synergy` to check value alignment, and `assess_intensity_resilience` to predict burnout risk based on program rigor.


## Available Tools (4)
- **analyze_coaching_match**: Specifically isolates how a founder's temperament interacts with different mentorship approaches
- **calculate_fit_score**: Provides a high-level assessment of how well a founder or team matches a specific accelerator program
- **evaluate_culture_synergy**: Determines if the founder's individual values will survive or thrive within the accelerator's ecosystem
- **assess_intensity_resilience**: Evaluates if the founder has the necessary psychological stamina for the program's specific rigor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Founder Personality Fit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fit score for a founder with traits ['resilient', 'structured'] for a program with culture ['high-growth', 'competitive'] using a 'directive' coaching style and intensity of 80."

**🤖 AI Agent:**
> The aggregate fit score is 75. Coaching compatibility is 85 due to the structured nature of the founder matching the directive style, while culture alignment is 65 due to the high intensity requirements.

---

**👤 You:**
> "Analyze the coaching match for a founder with traits ['creative', 'autonomous'] for a 'hands-off' coaching style."

**🤖 AI Agent:**
> The compatibility score is 90. The ideal style for this founder is hands-off, as their autonomy aligns perfectly with minimal supervision.

---

**👤 You:**
> "Evaluate the culture synergy for a founder with traits ['collaborative', 'community-focused'] in a program with culture ['individualistic', 'fast-paced']."

**🤖 AI Agent:**
> The alignment score is 40. Potential tension risks include a clash between the founder's community-focused nature and the program's individualistic environment.


## ❓ FAQ

**Q: What does the fit score represent?**
The fit score is a composite metric (0-100) representing the probability of success based on the intersection of founder traits, program culture, and coaching style.

**Q: How can I check if a founder will handle a high-pressure program?**
You can use the `assess_intensity_resilience` tool to evaluate if a founder's psychological profile can absorb the specific pressure and speed of the program.

**Q: Can this tool analyze entire founding teams?**
Yes, the `calculate_fit_score` tool accounts for team dynamics if multiple traits are provided in the input array.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-founder-personality-fit](https://vinkius.com/ai-agent-connect/accelerator-founder-personality-fit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Founder Personality Fit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-founder-personality-fit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Founder Personality Fit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-founder-personality-fit": {
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
