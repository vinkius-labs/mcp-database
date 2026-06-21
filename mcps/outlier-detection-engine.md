# Outlier Detection Engine MCP Server

Identify statistical anomalies in massive datasets local using deterministic Z-Score and IQR methods. Stop LLMs from guessing which rows are outliers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/outlier-detection-engine)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Outlier Detection Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outlier-detection-engine](https://vinkius.com/mcp/outlier-detection-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
