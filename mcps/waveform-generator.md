# Waveform Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/waveform-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Generate high-fidelity digital audio waveforms and noise profiles.

## Description
A mathematical engine for generating precise digital audio samples. Use `generate_periodic_wave` for sine, square, sawtooth, or triangle waves; `generate_noise_wave` for white or pink noise; and `generate_harmonic_wave` to build complex timbres using additive synthesis with custom harmonic series.


## Available Tools (3)
- **generate_periodic_wave**: Generates standard periodic waveforms (sine, square, sawtooth, or triangle)
- **generate_harmonic_wave**: Generates a custom waveform by summing harmonics
- **generate_noise_wave**: Generates non-periodic stochastic waveforms (white or pink noise)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waveform Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 2-second sine wave at 440Hz with an amplitude of 0.5."

**🤖 AI Agent:**
> The sine wave has been generated successfully, containing 88200 samples.

---

**👤 You:**
> "Create some pink noise for a 5-second duration at 48000Hz."

**🤖 AI Agent:**
> The pink noise generation is complete, providing 240000 samples of stochastic audio data.

---

**👤 You:**
> "Build a complex sound using harmonics: fundamental 220Hz, with a second harmonic at ratio 2 and amplitude 0.5."

**🤖 AI Agent:**
> The additive waveform was generated successfully with the specified harmonic series.


## ❓ FAQ

**Q: What types of waveforms can I generate?**
You can generate periodic waves (sine, square, sawtooth, triangle), stochastic noise (white, pink), and custom additive waveforms using `generate_harmonic_wave`.

**Q: Can I apply an amplitude envelope to the waves?**
Yes, all tools support an `envelopeConfig` parameter for ADSR (Attack, Decay, Sustain, Release) with linear or exponential curves.

**Q: How do I specify the sample rate?**
You can provide a `sampleRate` parameter (defaults to 44100 Hz) in any of the generation tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/waveform-generator](https://vinkius.com/mcp/waveform-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waveform Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waveform-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waveform Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waveform-generator": {
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
