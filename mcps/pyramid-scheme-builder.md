# Pyramid Scheme Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pyramid-scheme-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Generate and compare training repetition sequences using pyramidal progression.

## Description
The Pyramid Scheme Builder is a specialized tool for strength athletes and fitness enthusiasts to plan progressive overload sessions. It calculates the exact sequence of repetitions for ascending, peak (with optional multiple sets), and descending phases based on your target peak reps and step increment. Use `generate_pyramidal_sequence` to see your full workout volume, `validate_scheme_parameters` to ensure your progression is mathematically sound, or `compare_scheme_intensities` to evaluate which training structure provides the highest total workload.


## Available Tools (3)
- **compare_scheme_intensities**: Compares two different pyramid schemes to determine which generates more total work
- **generate_pyramidal_sequence**: Generates the complete list of repetitions for a specific training session and calculates total work
- **validate_scheme_parameters**: Verifies if a proposed set of training parameters is mathematically valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pyramid Scheme Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a pyramid sequence with 10 peak reps and an increment of 2."

**🤖 AI Agent:**
> The sequence is: 2, 4, 6, 8, 10, 8, 6, 4, 2. Total volume: 50 repetitions.

---

**👤 You:**
> "Calculate a pyramid with 6 peak reps, increment of 1, and 2 peak sets."

**🤖 AI Agent:**
> The sequence is: 1, 2, 3, 4, 5, 6, 6, 5, 4, 3, 2, 1. Total volume: 37 repetitions.

---

**👤 You:**
> "Compare a scheme with peak 5/inc 1 vs peak 10/inc 2."

**🤖 AI Agent:**
> The second scheme (peak 10, increment 2) is heavier. The volume difference is 25 repetitions.


## ❓ FAQ

**Q: What is a pyramid scheme in training?**
In this context, it refers to a set of repetitions that increases by a fixed amount until a peak is reached, then decreases back to the starting value.

**Q: How do I use the sequence generator?**
Use the `generate_pyramidal_sequence` tool by providing your target peak reps and the step increment you want to use for each set.

**Q: Can I repeat the top of the pyramid?**
Yes, by using the `peakSets` parameter in the generator, you can specify how many times to hold the maximum repetition count before starting the descent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pyramid-scheme-builder](https://vinkius.com/mcp/pyramid-scheme-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pyramid Scheme Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pyramid-scheme-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pyramid Scheme Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pyramid-scheme-builder": {
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
