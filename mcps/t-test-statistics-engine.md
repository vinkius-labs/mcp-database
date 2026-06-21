# T-Test Statistics Engine MCP Server

Run exact Student's, Welch's, and Paired t-tests local. Get CPU-guaranteed p-values instead of LLM-hallucinated guesses.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/t-test-statistics-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
LLMs are notoriously bad at math. If you ask an AI to calculate a p-value for a dataset, it will likely hallucinate a plausible-looking but completely wrong number. Data Scientists cannot tolerate this.

This MCP brings deterministic statistical computation to your AI. It delegates the complex math (Student's t-test, Welch's t-test, Paired t-tests) to the robust local `jstat` engine. The AI simply extracts the data, sends it to this engine, and gets back the mathematically guaranteed t-score, degrees of freedom, and exact p-value.

### The Superpowers

- **Zero Hallucination:** Exact p-values calculated by a CPU, not a language model.
- **Full T-Test Suite:** Supports Independent, Paired, and One-Sample tests.
- **Data Privacy:** Your company's experimental data stays local.
- **Automated Interpretation:** Automatically tells the AI whether to reject the null hypothesis at alpha=0.05.


## Available Tools
- **calculate_t_test**: Perform exact deterministic Student's t-tests (independent, paired, one-sample) to calculate statistical significance without LLM hallucinations


## Installation & Usage

To install and use the **T-Test Statistics Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/t-test-statistics-engine](https://vinkius.com/mcp/t-test-statistics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
