# Flexibility Score Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flexibility-score-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess flexibility using sit-and-reach measurements and demographic norms.

## Description
This MCP server provides a specialized engine to convert physical sit-and-reach measurements into standardized flexibility profiles. By using `calculate_flexibility_status`, users can obtain percentile rankings, flexibility categories, and identify tight muscle groups. The server also includes `get_stretching_guidance` to provide tailored movement recommendations based on assessment results.


## Available Tools (4)
- **calculate_flexibility_status**: Evaluates a single test attempt to provide a comprehensive flexibility profile
- **get_demographic_norm_range**: Retrieves the expected reach range for a specific demographic group
- **get_stretching_guidance**: Provides specific stretching protocols based on the assessment outcome
- **map_category_to_label**: Converts a numerical percentile into a human-readable flexibility classification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flexibility Score Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assess my flexibility: I reached 35cm, I am 25 years old, and I am female."

**🤖 AI Agent:**
> Your flexibility is in the 65th percentile, which is categorized as Average. Your hamstrings show slight tightness. We recommend the 'Lower Body Mobility' routine with moderate intensity.

---

**👤 You:**
> "What is the expected reach range for a 40-year-old male?"

**🤖 AI Agent:**
> For a 40-year-old male, the expected reach range is between 32cm and 41cm, with a mean of 36.5cm.

---

**👤 You:**
> "I am in the 15th percentile for flexibility. What should I do?"

**🤖 AI Agent:**
> Since you are in the 15th percentile, you should focus on the 'Foundation Flexibility' routine with low intensity to safely improve your range of motion.


## ❓ FAQ

**Q: What is the sit-and-reach test?**
It is a standard field test used to measure the flexibility of the lower back and hamstring muscles.

**Q: How do I use the stretching recommendations?**
After running `calculate_flexibility_status`, use the resulting muscle tightness data with `get_stretching_guidance` to receive a specific routine.

**Q: Can I use a modified test version?**
Yes, the `calculate_flexibility_status` tool includes an `isModifiedTest` parameter to account for non-standard test variations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flexibility-score-assessment](https://vinkius.com/en/ai-agent-connect/flexibility-score-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flexibility Score Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flexibility-score-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flexibility Score Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flexibility-score-assessment": {
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
