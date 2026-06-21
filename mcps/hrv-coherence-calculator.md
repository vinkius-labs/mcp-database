# HRV Coherence Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hrv-coherence-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hrv-coherence-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hrv-coherence-calculator-mcp)
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


## Installation & Usage

To install and use the **HRV Coherence Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hrv-coherence-calculator](https://vinkius.com/mcp/hrv-coherence-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
