# Signal Filter Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signal-filter-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Apply digital filters like low-pass, high-pass, SMA, EMA, and Peaking EQ to signal arrays.

## Description
The Signal Filter Designer MCP server provides a suite of digital signal processing (DSP) tools for manipulating one-dimensional numerical arrays. You can use `apply_first_order_filter` to remove high-frequency noise or low-frequency drift, `apply_moving_average_sma` to smooth short-term fluctuations, `apply_exponential_moving_average` for weighted smoothing, and `apply_peaking_eq` to boost or cut specific frequency ranges. It is ideal for processing sensor data, audio samples, or any time-series signal arrays.


## Available Tools (4)
- **apply_moving_average_sma**: Smooths out short-term fluctuations in data by averaging local data points
- **apply_peaking_eq**: Boosts or cuts specific frequency ranges to shape the signal's tone
- **apply_exponential_moving_average**: Smooths data while allowing for more recent changes to have a programmable impact on the output
- **apply_first_order_filter**: Cutoff must be below Nyquist limit.

Applies basic attenuation to remove either high-frequency noise or low-frequency drift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Signal Filter Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Apply a low-pass filter to this signal: [1, 2, 3, 4, 5, 4, 3, 2, 1] with a sample rate of 10Hz and a cutoff frequency of 2Hz."

**🤖 AI Agent:**
> [1.0, 1.5, 2.2, 2.8, 3.5, 3.2, 2.5, 1.8, 1.2]

---

**👤 You:**
> "Smooth this data using a moving average with a window size of 3: [10, 20, 30, 40, 50]."

**🤖 AI Agent:**
> [10.0, 20.0, 30.0, 40.0, 50.0]

---

**👤 You:**
> "Boost the frequency at 100Hz by 6dB using a peaking EQ on this signal: [0, 1, 0, -1, 0] with sample rate 400Hz and Q of 1.0."

**🤖 AI Agent:**
> [0.0, 1.2, 0.0, -1.2, 0.0]


## ❓ FAQ

**Q: What is the Nyquist limit?**
The Nyquist limit is half of your sample rate. Any frequency you attempt to filter using `apply_first_order_filter` or `apply_peaking_eq` must be below this value to ensure signal integrity.

**Q: Can I use this for audio processing?**
Yes, if you provide the correct sample rate. Tools like `apply_peaking_eq` are specifically designed to shape frequency responses in audio signals.

**Q: How does the smoothing factor work in EMA?**
In `apply_exponential_moving_average`, the alpha value (between 0 and 1) determines how much weight is given to the newest sample. A higher alpha makes it react faster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signal-filter-designer](https://vinkius.com/mcp/signal-filter-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Signal Filter Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `signal-filter-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Signal Filter Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "signal-filter-designer": {
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
