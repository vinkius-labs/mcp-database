# Emotion Wheel Classifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emotion-wheel-classifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emotion-wheel-classifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emotion-wheel-classifier-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [psychology](../categories/psychology.md)

Map raw text descriptions to Plutchik's Wheel of Emotions, identifying intensity and emotional families.

## Description
The Emotion Wheel Classifier connects AI agents to the psychological depth of Plutchik's model. Use `analyze_text_emotion` to transform unstructured text into specific emotional nodes, intensities (Low, Medium, High), and families. You can also use `get_emotion_spectrum` to see how an emotion evolves in strength or `explore_emotional_dyad` to calculate the complex emotions resulting from combining two primary states.


## Available Tools
- **explore_emotional_dyad**: Calculate the resulting complex emotion from two primary emotions
- **get_emotion_spectrum**: Show the progression of a specific emotion
- **analyze_text_emotion**: Analyze raw text to identify emotion, intensity, and family


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emotion Wheel Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I feel extremely happy and full of energy!"

**🤖 AI Agent:**
> The `analyze_text_emotion` tool identifies the primary emotion as Joy with a High intensity level.

---

**👤 You:**
> "I am slightly afraid of the dark."

**🤖 AI Agent:**
> The `analyze_text_emotion` tool identifies the primary emotion as Fear with a Low intensity level.

---

**👤 You:**
> "What happens if I combine Joy and Trust?"

**🤖 AI Agent:**
> Using `explore_emotional_dyad` with Joy and Trust results in the complex emotion of Love.


## Installation & Usage

To install and use the **Emotion Wheel Classifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emotion-wheel-classifier](https://vinkius.com/mcp/emotion-wheel-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
