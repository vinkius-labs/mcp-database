# YAML/JSON Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yamljson-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yamljson-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yamljson-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Prevent DevOps YAML hallucination. Convert complex YAML files to JSON for safe AI processing, and back to perfect YAML.

## Description
LLMs struggle with YAML. Because YAML relies strictly on whitespace indentation, an autoregressive language model often misaligns keys when generating massive Kubernetes manifests or GitHub Actions. This MCP solves that by converting YAML to JSON (which LLMs handle perfectly) and dumping JSON back to strictly-formatted YAML.

### The Superpowers

- **Indentation Protection:** Uses `js-yaml` to ensure every space is perfectly aligned when writing files.
- **Bi-directional:** Seamlessly swap between `yaml2json` and `json2yaml` for DevOps and CI/CD agentic workflows.


## Available Tools
- **convert_yaml**: Pass the source string and the desired direction. The engine handles complex nested structures, arrays, and multiline values deterministically.

Converts massive YAML files to JSON and vice-versa, preventing indentation hallucinations by the LLM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YAML/JSON Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this Kubernetes deployment YAML into JSON so I can safely read the environment variables."

**🤖 AI Agent:**
> ✅ **Converted to JSON:** Payload correctly mapped with zero indentation errors.

---

**👤 You:**
> "Dump this JSON configuration object back into `json2yaml` format with strict 2-space indentation."

**🤖 AI Agent:**
> ✅ **YAML Output:** Correctly formatted YAML string ready to be saved.


## Installation & Usage

To install and use the **YAML/JSON Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yamljson-converter](https://vinkius.com/mcp/yamljson-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
