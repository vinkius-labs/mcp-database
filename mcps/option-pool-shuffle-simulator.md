# Option Pool Shuffle Simulator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/option-pool-shuffle-simulator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/option-pool-shuffle-simulator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/option-pool-shuffle-simulator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze the dilution impact of option pool timing during VC investment rounds.

## Description
This simulator helps founders understand the true cost of the 'Option Pool Shuffle'. By comparing `compute_pre_money_scenario` and `compute_post_money_scenario`, you can see exactly how much equity is lost when an ESOP is negotiated as post-money versus pre-money. Use `compare_shuffle_impact` to calculate the precise percentage delta and monetary value loss in your next funding round.


## Available Tools
- **compute_post_money_scenario**: Calculates ownership when the option pool is created post-investment
- **compare_shuffle_impact**: Compares pre-money vs post-money scenarios to reveal the cost of the shuffle
- **compute_pre_money_scenario**: Calculates ownership when the option pool is part of the pre-money valuation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Option Pool Shuffle Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ownership if I have a $5M pre-money valuation, a $2M investment, and want a 10% option pool."

**🤖 AI Agent:**
> In the pre-money scenario, your post-money valuation is $7M. The founders will hold approximately 64.29% of the company after accounting for both the investor's stake and the 10% option pool.

---

**👤 You:**
> "What happens to my ownership if the investor insists on a post-money option pool?"

**🤖 AI Agent:**
> In the post-money scenario, the dilution is higher for founders. The tool shows that your ownership percentage decreases because the expansion of the pool occurs after the investment, protecting the investor's stake.

---

**👤 You:**
> "Compare the impact of a $1M loss in equity value."

**🤖 AI Agent:**
> The comparison reveals that the 'shuffle' results in a specific percentage point delta and a measurable monetary loss based on your company's valuation, which you can use as leverage in negotiations.


## Installation & Usage

To install and use the **Option Pool Shuffle Simulator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/option-pool-shuffle-simulator](https://vinkius.com/mcp/option-pool-shuffle-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
