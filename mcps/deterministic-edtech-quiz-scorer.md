# Deterministic EdTech Quiz Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-edtech-quiz-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform your AI into a ruthless, high-precision EdTech examiner. Automatically cross-reference quiz answers against weighted keys to generate granular performance metrics instantly.

## Description
Building custom assessment pipelines usually involves writing bloated scripts to compare arrays, calculate weighted averages, and isolate category weaknesses. The EdTech Quiz Scorer MCP solves this by offloading the entire grading pipeline to a hyper-optimized V8 algorithmic engine.

### The Superpowers
- **Granular Category Analytics:** It doesn't just give a final score. It breaks down the exam by `category` (e.g., 'Math', 'Science'), revealing exactly where the student's weaknesses lie.
- **Weighted Scoring Framework:** Supports dynamic weighting. A difficult question can be worth 5 points while a true/false is worth 1 point. The engine perfectly calculates the max possible score and percentage.
- **Speed & Time Tracking:** Ingests the total time taken and automatically derives the `averageTimePerQuestionSeconds`, a critical metric for standardized test preparation.
- **Zero-Dependency Architecture:** Pure JS runtime execution guarantees absolute microsecond speed without any massive external EdTech NPM dependencies. Perfect for real-time agentic evaluation workflows.


## Available Tools (1)
- **score_quiz**: You must provide the answerKeyStr and userAnswersStr as stringified JSON arrays. Optionally provide totalTimeSeconds to calculate time metrics.

Automatically cross-references a user's quiz answers against a weighted answer key, generating granular EdTech performance metrics and categorical accuracy percentages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic EdTech Quiz Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Score this 10-question Math exam for the student."

**🤖 AI Agent:**
> Using the score_quiz tool: The student scored 8.5 out of 10.0 (85% accuracy). They missed questions #3 and #7.

---

**👤 You:**
> "Give me a category breakdown of the student's weaknesses."

**🤖 AI Agent:**
> Using the score_quiz tool: The category breakdown shows the student excels in 'Algebra' (100%), but is struggling in 'Geometry' (only 40% correct).

---

**👤 You:**
> "Calculate the average time per question if they finished in 180 seconds."

**🤖 AI Agent:**
> Using the score_quiz tool (totalTimeSeconds=180): The performance metrics show an average of 18 seconds spent per question.


## ❓ FAQ

**Q: Why should I use an MCP instead of asking the AI to grade it?**
LLMs hallucinate math. If you give an LLM 50 questions, it will often miscount the correct answers, fail to apply fractional weights, or hallucinate the final percentage. This MCP uses deterministic V8 loops, guaranteeing 100% mathematical accuracy.

**Q: How does the weighting system work?**
In your `answerKey` JSON array, you can add a `weight` parameter (e.g., `weight: 2.5`). The engine automatically tallies the `maxPossibleScore` and evaluates the user's earned points against it, rather than just doing a flat 1-point-per-question calculation.

**Q: Does it track which questions the user got wrong?**
Yes. The output payload includes an array called `incorrectQuestionIds`, which isolates the exact IDs the user failed, allowing your AI to instantly provide targeted tutoring on those specific topics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-edtech-quiz-scorer](https://vinkius.com/mcp/deterministic-edtech-quiz-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic EdTech Quiz Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-edtech-quiz-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic EdTech Quiz Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-edtech-quiz-scorer": {
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
