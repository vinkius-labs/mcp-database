# Text Readability Scorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/text-readability-scorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/text-readability-scorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/text-readability-scorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate mathematically accurate readability metrics (Flesch-Kincaid, Gunning Fog, SMOG) for any text. Stop relying on AI 'feelings' — get exact US grade levels for SEO and compliance.

## Description
You ask your AI copywriter: 'Is this blog post easy to read?' It says 'Yes, it is very engaging!' Then you run it through a real SEO tool and it scores at a university reading level — killing your mobile bounce rate.

LLMs cannot accurately count syllables or calculate sentence complexity. This MCP uses the `text-readability` library to execute standard linguistic formulas, providing mathematical proof of how difficult your text is to read.

### The Superpowers

- **Flesch-Kincaid Grade Level:** The industry standard. Returns a number corresponding to the US grade level (e.g., 8.2 = 8th grade).
- **Flesch Reading Ease:** A 0-100 scale where higher is easier. Essential for broad audience copy.
- **Multiple Algorithms:** Also calculates Gunning Fog, Coleman-Liau, SMOG, and Automated Readability Index (ARI).
- **Consensus Evaluation:** Automatically aggregates all scores to give you a definitive target audience level.


## Available Tools
- **readability_scorer**: Essential for SEO, marketing, and legal compliance.

Calculate rigorous readability metrics for any text (Flesch-Kincaid, Gunning Fog, SMOG, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Text Readability Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this landing page copy. We need it to be at an 8th-grade reading level to maximize conversions."

**🤖 AI Agent:**
> Flesch-Kincaid Grade: 11.4 | Reading Ease: 42.1 | Consensus: 11th and 12th grade. Too complex. Needs simplification.

---

**👤 You:**
> "Our legal team says the new Terms of Service must be readable by a 6th grader. Verify the text."

**🤖 AI Agent:**
> Flesch-Kincaid Grade: 6.2 | Reading Ease: 78.5 | Meets compliance requirement for 6th-grade readability.

---

**👤 You:**
> "Check the SMOG Index and Gunning Fog for this medical article before we publish it."

**🤖 AI Agent:**
> SMOG: 14.2 | Gunning Fog: 15.8 | Highly academic. Requires college-level reading comprehension.


## Installation & Usage

To install and use the **Text Readability Scorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/text-readability-scorer](https://vinkius.com/mcp/text-readability-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
