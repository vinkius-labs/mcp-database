# Meditation Session Planner MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meditation-session-planner)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/meditation-session-planner-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/meditation-session-planner-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Get a structured meditation plan tailored to your time and mental goal, complete with phase guidance.

## Description
**Need structure for deep rest?** Meditation can feel unstructured. Many users struggle knowing *how* to start or how long each part should be. The goal is always insight, but the process requires planning.


## Available Tools
- **allocate_durations**: Minimum 5, maximum 60 minutes.

Allocate time durations for meditation session phases
- **get_practice_guidance**: Valid phases: Grounding, Core Practice, Integration.

Get detailed practice guidance for a specific meditation phase and goal
- **plan_session**: Valid goals are: focus, sleep, anxiety, self-awareness.

Plan a meditation session based on the user's goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meditation Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 20 minutes available. My main goal is improving focus on work tasks."

**🤖 AI Agent:**
> First, run `plan_session` with goal='focus'. Next, use `allocate_durations` for totalMinutes=20. Finally, call `get_practice_guidance` using the resulting phases and 'focus' as context to get detailed instructions.

---

**👤 You:**
> "I am highly anxious right now and only have 10 minutes. Give me a plan."

**🤖 AI Agent:**
> Start by running `plan_session` with goal='anxiety'. Then, use `allocate_durations` for totalMinutes=10. The output will guide you on how to proceed immediately using `get_practice_guidance`.

---

**👤 You:**
> "I want a gentle session for sleep, and I have 45 minutes. Plan it out."

**🤖 AI Agent:**
> Use `plan_session` with goal='sleep' to get the ideal structure. Run `allocate_durations` for totalMinutes=45. Then, use `get_practice_guidance` on each phase name that results.


## Installation & Usage

To install and use the **Meditation Session Planner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meditation-session-planner](https://vinkius.com/mcp/meditation-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
