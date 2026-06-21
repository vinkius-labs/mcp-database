# HRV Coherence Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hrv-coherence-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates key Heart Rate Variability (HRV) metrics (RMSSD, SDNN) to classify cardiorespiratory coherence level using R-R intervals.

## Description
**The Problem:** Understanding heart rate variability (HRV) is critical for assessing the body's autonomic nervous system balance. Raw measurements of successive R-R intervals can be complex to interpret, especially when determining if the overall cardiovascular system coherence is optimal or reduced.


## Available Tools
- **classify_coherence_level**: Classify cardiorespiratory coherence level based on HRV metrics
- **calculate_rmssd**: Requires at least 3 readings.

Calculate RMSSD from R-R intervals
- **calculate_sdnn**: Requires at least 5 readings for statistical reliability.

Calculate SDNN from R-R intervals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HRV Coherence Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have R-R intervals: [1000, 950, 1020, 1100]. My age is 30 and I am Male. Please calculate my coherence."

**🤖 AI Agent:**
> First, I will run `calculate_rmssd` to get the short-term measure. Then, I'll use the resulting RMSSD and any available SDNN value with `classify_coherence_level`, providing my age (30) and sex (Male), to give a full coherence assessment.

---

**👤 You:**
> "Calculate the overall variability for this long set of R-R data: [1200, 1150, 1300, 1400, 1280]."

**🤖 AI Agent:**
> I recommend using the `calculate_sdnn` tool for this overall variability measure. Once you have both SDNN and RMSSD, remember to pass them together into the `classify_coherence_level` function along with your demographics.

---

**👤 You:**
> "I need a full coherence report. My age is 45 and I am Female. The metrics are RMSSD: 35ms and SDNN: 80ms."

**🤖 AI Agent:**
> Running the `classify_coherence_level` tool with your provided data (RMSSD=35, SDNN=80, Age=45, Sex=Female) will generate a detailed report on your cardiorespiratory coherence level.


## ❓ FAQ

**Q: What is the difference between RMSSD and SDNN?**
RMSSD measures short-term variation (parasympathetic activity), while SDNN assesses total variability. Both metrics are calculated using dedicated tools: `calculate_rmssd` for the former and `calculate_sdnn` for the latter.

**Q: Do I need to provide age and sex?**
Yes. The classification of your coherence level requires demographic context. The `classify_coherence_level` tool uses your age and sex to compare calculated metrics against established physiological norms.

**Q: What are the minimum requirements for input data?**
Data constraints vary by metric. `calculate_rmssd` requires a minimum of 3 readings, and `calculate_sdnn` requires at least 5 readings to ensure statistical reliability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hrv-coherence-calculator](https://vinkius.com/mcp/hrv-coherence-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HRV Coherence Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hrv-coherence-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HRV Coherence Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hrv-coherence-calculator": {
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
