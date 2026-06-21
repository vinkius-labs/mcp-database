# HrFlow.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hrflowai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hrflowai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hrflowai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI-powered talent acquisition API for parsing, matching, and reasoning.

## Description
Empower your AI agents with HrFlow.ai's advanced talent acquisition capabilities. This MCP server allows you to parse resumes, search profiles and jobs with semantic filters, score candidates against job descriptions, and ask natural language questions about profiles. Ideal for automating recruitment workflows with AI-driven insights.


## Available Tools
- **ask_profile**: Asks a natural language question about a specific profile
- **list_boards**: Lists job boards
- **list_jobs**: Lists jobs stored in HrFlow boards
- **list_profiles**: Lists candidate profiles stored in HrFlow
- **list_sources**: Lists profile sources
- **parse_profile**: Parses a resume file into a structured profile
- **score_profiles**: Scores candidate profiles against a specific job
- **search_jobs**: Searches for jobs with semantic filters
- **search_profiles**: Searches for profiles with semantic filters
- **unfold_profile**: Analyzes and unfolds the career path of a profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HrFlow.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 profiles added to my HrFlow source."

**🤖 AI Agent:**
> I'll fetch the latest profiles for you.

---

**👤 You:**
> "Ask profile key 'abc-123' if they have experience with Kubernetes."

**🤖 AI Agent:**
> I'll analyze the candidate's profile and answer your question.

---

**👤 You:**
> "Find jobs that match candidate 'john-doe-key'."

**🤖 AI Agent:**
> I'll use semantic search to find matching jobs for this candidate.


## Installation & Usage

To install and use the **HrFlow.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hrflowai](https://vinkius.com/mcp/hrflowai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
