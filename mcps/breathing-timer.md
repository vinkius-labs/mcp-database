# Breathing Timer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/breathing-timer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/breathing-timer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/breathing-timer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Accurately track structured breathing cycles (Box Breathing, 4-7-8, Coherence Heart Rate) for guided respiratory practice.

## Description
Feeling stressed or needing to reset your focus? Controlled breathing is a foundational skill in managing the autonomic nervous system. The problem is that maintaining precise, measured breath patterns--like Box Breathing (4-4-4-4) or 4-7-8--requires perfect timing and counting. Our application provides structure and accuracy.

Mechanism: This MCP connects your agents to core physiological rhythm tracking. It uses three primary tools:
1. `query_breathing_parameters`: Retrieves the scientifically backed default timings for techniques like Coherence Heart Rate or Wim Hof.
2. `calculate_single_cycle_duration`: Determines the precise time needed for one full cycle based on user inputs (e.g., 4s Inhale, 7s Hold, 8s Exhale).
3. `generate_breathing_schedule`: Takes your desired total session length and counts down in structured cycles, providing moment-by-moment guidance.

The advantage is a reliable, guided practice that allows you to focus entirely on the breath, knowing the timing structure is flawless.


## Available Tools
- **calculate_single_cycle_duration**: Calculate the total duration of one full breathing cycle for a given technique
- **query_breathing_parameters**: Query the default timing parameters for a breathing technique
- **generate_breathing_schedule**: Generate a structured breathing schedule for a given total duration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breathing Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a 15-minute session using the 4-7-8 technique. Start now."

**🤖 AI Agent:**
> Okay, starting your 15-minute 4-7-8 cycle schedule. The first phase is INHALE (count of 4). Remember to breathe deeply and consistently. We will continue the pattern for the next 15 minutes.

---

**👤 You:**
> "What are the standard timing parameters for Coherence Heart Rate?"

**🤖 AI Agent:**
> According to our catalog, the default parameters for Coherence Heart Rate (COHERENT) are: Inhale: 5 seconds, Hold After Inhale: 0 seconds, Exhale: 5 seconds, Rest: 0 seconds. This means one full cycle takes 10 seconds.

---

**👤 You:**
> "Calculate the duration for a custom Box Breathing cycle using 3s inhale and 5s exhale."

**🤖 AI Agent:**
> I have calculated your customized Box Breathing cycle duration. With 3 seconds inhale, 3 seconds hold, 5 seconds exhale, and 3 seconds rest, one full cycle will take a total of 14 seconds.


## Installation & Usage

To install and use the **Breathing Timer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/breathing-timer](https://vinkius.com/mcp/breathing-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
