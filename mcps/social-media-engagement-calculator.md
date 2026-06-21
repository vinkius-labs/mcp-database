# Social Media Engagement Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/social-media-engagement-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/social-media-engagement-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/social-media-engagement-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate platform-specific engagement rates for Instagram and LinkedIn and compare them against industry benchmarks.

## Description
This MCP server provides specialized tools to quantify social media performance. Use `compute_instagram_engagement` to calculate engagement rates based on likes, comments, and saves relative to impressions. Use `compute_linkedin_engagement` to determine LinkedIn engagement using likes, comments, and shares. You can also use `retrieve_benchmark_standard` to find the target engagement rate for specific account tiers like Nano, Micro, Macro, or Mega.


## Available Tools
- **retrieve_benchmark_standard**: Retrieves the target engagement benchmark for a specific account size tier
- **compute_instagram_engagement**: Determines the engagement rate for Instagram posts
- **compute_linkedin_engagement**: Determines the engagement rate for LinkedIn posts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Media Engagement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my Instagram engagement rate for a post with 100 likes, 20 comments, 5 saves, and 1000 impressions."

**🤖 AI Agent:**
> The calculated Instagram engagement rate is 12.5%.

---

**👤 You:**
> "What is the benchmark for a Micro account?"

**🤖 AI Agent:**
> The target engagement rate for a Micro account tier is 3.5%.

---

**👤 You:**
> "Check LinkedIn engagement: 50 likes, 10 comments, 5 shares, and 500 impressions."

**🤖 AI Agent:**
> The calculated LinkedIn engagement rate is 13.0%.


## Installation & Usage

To install and use the **Social Media Engagement Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/social-media-engagement-calculator](https://vinkius.com/mcp/social-media-engagement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
