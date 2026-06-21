# Outlier Detection Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/outlier-detection-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/outlier-detection-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/outlier-detection-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Identify statistical anomalies in massive datasets local using deterministic Z-Score and IQR methods. Stop LLMs from guessing which rows are outliers.

## Description
Outliers skew machine learning models and corrupt statistical analysis. If you ask an LLM to scan 10,000 rows for anomalies, it will exhaust its context and arbitrarily flag random rows based on visual intuition — not math.

This MCP delegates outlier detection to `simple-statistics`. The engine calculates exact Means, Standard Deviations, and Quartiles, then flags specific rows mathematically using Z-Score or IQR bounds. No intuition, no guessing — just pure deterministic statistics.

### The Superpowers

- **Mathematical Precision:** Every flagged outlier comes with its exact Z-Score or IQR boundary values.
- **Multiple Methods:** Choose Z-Score (parametric, best for normal distributions) or IQR (robust, best for skewed data).
- **Customizable Threshold:** Set your own sensitivity (Z > 3, IQR × 1.5, etc.).
- **High Performance:** Scans thousands of rows instantly on your local machine.


## Available Tools
- **detect_outliers**: Deterministically identify statistical outliers in datasets using Z-Score or IQR methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outlier Detection Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all rows where the 'Temperature' reading is a statistical outlier using Z-Score > 3."

**🤖 AI Agent:**
> Found 4 outliers. The most extreme is row 142 with Temperature 98.5°C (Z-Score = 4.1), followed by row 87 (Z = 3.8), row 201 (Z = 3.4), and row 15 (Z = 3.1).

---

**👤 You:**
> "Check the 'Price' column for anomalies using the robust IQR method with a 1.5 multiplier."

**🤖 AI Agent:**
> Using an IQR threshold of 1.5, I identified 12 items priced significantly above the upper bound of $450 (Q3 + 1.5×IQR). These appear to be luxury or premium-tier products.

---

**👤 You:**
> "Are there any abnormal network latency values in this monitoring dataset?"

**🤖 AI Agent:**
> Yes. Using Z-Score analysis, 3 network requests had ping times exceeding 3 standard deviations (Z > 3): rows 44 (Z=3.9), 128 (Z=3.5), and 302 (Z=3.2).


## Installation & Usage

To install and use the **Outlier Detection Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outlier-detection-engine](https://vinkius.com/mcp/outlier-detection-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
