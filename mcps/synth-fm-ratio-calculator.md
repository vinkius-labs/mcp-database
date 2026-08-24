# Synth FM Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/synth-fm-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

A deterministic FM synthesis engine for calculating harmonic ratios and sideband spectra.

## Description
This MCP server provides a deterministic Frequency Modulation (FM) synthesis engine. It allows AI agents to calculate the mathematical relationship between carrier and modulator frequencies, classify spectra as harmonic or inharmonic, and generate detailed sideband distributions. Use `analyze_fm_ratio` to find the C:M ratio, `calculate_sideband_spectrum` to map frequency/amplitude distributions, and `identify_audible_frequencies` to filter sidebands based on a specific amplitude threshold.


## Available Tools (3)
- **analyze_fm_ratio**: Determines the mathematical relationship between the carrier and modulator to classify the resulting sound type
- **calculate_sideband_spectrum**: Generates a detailed list of the frequencies and relative amplitudes of the sidebands produced by the modulation
- **identify_audible_frequencies**: Filters a spectrum to identify only those sidebands that possess sufficient amplitude to be perceived


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Synth FM Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the C:M ratio for a carrier of 440Hz and a modulator of 220Hz?"

**🤖 AI Agent:**
> The C:M ratio is 2:1, and the resulting spectrum is harmonic.

---

**👤 You:**
> "Calculate the sideband spectrum for a 440Hz carrier, 110Hz modulator, and 2.0 modulation index."

**🤖 AI Agent:**
> The sidebands include the carrier at 440Hz, and sidebands at 330Hz, 550Hz, 220Hz, 660Hz, 110Hz, and 770Hz with their respective calculated amplitudes.

---

**👤 You:**
> "Which frequencies are audible if the threshold is 0.1 for a 440Hz carrier and 220Hz modulator with index 1.5?"

**🤖 AI Agent:**
> The audible frequencies above the 0.1 threshold are 440Hz, 220Hz, and 660Hz.


## ❓ FAQ

**Q: What is the difference between harmonic and inharmonic spectra?**
Harmonic spectra occur when the C:M ratio consists of simple integer relationships, resulting in musical tones. Inharmonic spectra occur when the ratio is complex or irrational, creating bell-like or metallic sounds.

**Q: How are sideband amplitudes calculated?**
Sideband amplitudes are determined by approximating Bessel functions of the first kind based on the provided modulation index.

**Q: Can I filter out quiet sidebands?**
Yes, you can use the `identify_audible_frequencies` tool to filter the spectrum for sidebands that exceed a specific amplitude threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/synth-fm-ratio-calculator](https://vinkius.com/ai-agent-connect/synth-fm-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Synth FM Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `synth-fm-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Synth FM Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "synth-fm-ratio-calculator": {
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
