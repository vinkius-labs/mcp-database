# Lead Time Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lead-time-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lead-time-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lead-time-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Analyze and decompose supply chain lead times to identify bottlenecks.

## Description
The Lead Time Analyzer is a specialized tool for supply chain professionals. It decomposes total lead time into specific stages, allowing you to distinguish between Value-Added and Non-Value-Added time. By using tools like `analyze_lead_time_composition`, you can identify the primary bottleneck in your process. Additionally, `calculate_reduction_impacts` allows you to simulate a 20% reduction in any stage to see its effect on the total duration, while `evaluate_process_volatility` helps you understand which stages contribute most to process uncertainty.


## Available Tools
- **analyze_lead_time_composition**: Calculates the core metrics of the lead time breakdown
- **calculate_reduction_impacts**: Simulates efficiency gains by optimizing specific stages
- **evaluate_process_volatility**: Determines which stages contribute most to the unpredictability of the total lead time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lead Time Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my lead time: Order Processing is 2h, Production/Picking is 5h, Transport is 10h, Receiving is 3h, and Inspection is 2h."

**🤖 AI Agent:**
> The total lead time is 22 hours. The bottleneck stage is Transport (10h). Value-Added time is 5h, and Non-Value-Added time is 17h.

---

**👤 You:**
> "What happens to my total lead time if I reduce the Transport stage by 20%?"

**🤖 AI Agent:**
> If you reduce the Transport stage from 10h to 8h, your new total lead time will be 20 hours, resulting in a reduction of 2 hours.

---

**👤 You:**
> "Which stage contributes most to the variability of my process? (Deviations: Order Processing: 0.5, Production/Picking: 1, Transport: 3, Receiving: 0.2, Inspection: 0.1)"

**🤖 AI Agent:**
> The stage contributing most to the process volatility is Transport.


## Installation & Usage

To install and use the **Lead Time Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lead-time-analyzer](https://vinkius.com/mcp/lead-time-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
