# Content Length Benchmark Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/content-length-benchmark-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-analysis](../categories/content-analysis.md)

Analyze copy length, density, and structural scannability against established copywriting benchmarks.

## Description
The Content Length Benchmark Analyzer evaluates how well your text adheres to optimal word counts and structures for various marketing formats. Use `get_text_metrics` to extract fundamental linguistic counts like word, sentence, and paragraph totals. For specific content types like 'Blog Intro' or 'Landing Page Hero', use `check_benchmark_deviations` to identify percentage deviations from target ranges. Additionally, utilize `analyze_scannability` to assess text breathability and mobile optimization by analyzing paragraph length distribution.


## Available Tools (3)
- **analyze_scannability**: Analyzes text scannability for mobile
- **check_benchmark_deviations**: Compares text metrics against benchmarks
- **get_text_metrics**: Extracts linguistic metrics from raw text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Content Length Benchmark Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the basic metrics for this text: 'Hello world. This is a test paragraph.'"

**🤖 AI Agent:**
> Word count: 8, Sentence count: 2, Paragraph count: 1.

---

**👤 You:**
> "Check if a Blog Intro with 150 words, 10 sentences, and 3 paragraphs is within the benchmark range."

**🤖 AI Agent:**
> The metrics are within the allowed deviation buffer for a Blog Intro.

---

**👤 You:**
> "Analyze the scannability of paragraphs with lengths [10, 50, 200] and a line break frequency of 2."

**🤖 AI Agent:**
> The distribution ratio shows a mix of short, medium, and long paragraphs. The mobile scannability check passed.


## ❓ FAQ

**Q: What metrics can I extract from my text?**
Using the `get_text_metrics` tool, you can retrieve total word counts, sentence counts, paragraph counts, and line break frequency.

**Q: How does the analyzer handle different content types?**
The `check_benchmark_deviations` tool compares your text metrics against specific benchmarks for formats like Landing Page Hero, Blog Intro, and Email Body.

**Q: Can I check if my content is optimized for mobile reading?**
Yes, the `analyze_scannability` tool evaluates paragraph length distribution and white-space density to determine if your text meets mobile scannability thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/content-length-benchmark-analyzer](https://vinkius.com/mcp/content-length-benchmark-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Content Length Benchmark Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `content-length-benchmark-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Content Length Benchmark Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "content-length-benchmark-analyzer": {
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
