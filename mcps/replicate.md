# Replicate MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/replicate)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/replicate-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/replicate-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Equip your AI to dynamically search, run, and monitor thousands of open-source machine learning models hosted on Replicate via simple text commands.

## Description
Connect your conversational assistant directly to the **Replicate** ecosystem. This integration grants your AI the ability to interact programmatically with a vast library of open-source machine learning models without running them on your local hardware. From orchestrating complex image generations to spinning up specialized language models, you can command AI workflows directly from your chat.

### What you can do

- **Execute Predictions** — Command the assistant to execute specific model versions on your behalf (`create_prediction`) by supplying a payload of variables. Monitor long-running processes by retrieving outputs and execution status reliably (`get_prediction`) or cancel them at will (`cancel_prediction`).
- **Discover Models** — Instruct the AI to intelligently scan the Replicate platform for models matching a specific use case using `search_models`. You can also explore trending and categorized models by leveraging the `list_collections` action.
- **Analyze Model Metadata** — Whenever you discover a new model, query its precise owner and name (`get_model`) to extract the exact schema and parameter requirements necessary for a successful execution. You can also view a log of your own executed tasks (`list_predictions`).

### How it works

1. Install the Replicate platform extension module in your MCP.
2. Provide your personal `Replicate API Token`, extracted from your Replicate Account Settings panel. Deposit it securely into the configuration variables below.
3. Prompt your assistant organically: "Search for a high-quality video generation model, evaluate its parameter schema, and start generating a clip using the prompt 'a cat walking on Mars'."

### Who is this for?

- **AI Developers & Researchers** — Explore and test novel open-source algorithms by generating quick predictions without modifying Python notebook code.
- **Content Creators** — Execute specialized image, audio, or video generation tasks by directly delegating workflows to your conversational assistant.
- **Builders** — Mix and match the output of various specialized models intelligently using natural language instructions.


## Available Tools
- **list_models**: Lists public models available on Replicate
- **get_account**: Retrieves the authenticated Replicate account details
- **list_collections**: g., "Image-to-Text", "Audio Generation").

Lists curated collections of models
- **list_deployments**: Lists your active model deployments on Replicate
- **cancel_prediction**: Cancels a prediction that is currently running
- **create_prediction**: g., image generation, LLMs). Provide the model version ID and inputs as a JSON object.

Starts a new model prediction on Replicate
- **get_collection**: Provide the collection slug (e.g., "text-to-image").

Retrieves a specific collection of models by its slug
- **get_model**: Retrieves details for a specific model
- **get_prediction**: ).

Retrieves the status and output of a prediction
- **list_hardware**: Lists available GPU hardware options for running models
- **list_predictions**: Lists recent predictions made by the user
- **search_models**: Searches for public models on Replicate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Replicate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent predictions."

**🤖 AI Agent:**
> Invoking `list_predictions` has successfully found your last requests. The most recent executed instance has an ID of `p_30abc...`, which is confirmed finished, running a prompt about dog pictures.

---

**👤 You:**
> "Query Replicate to search for 'TTS' models."

**🤖 AI Agent:**
> I ran `search_models` using your keyword "TTS". Replicate returned a wide array of options, including 'suno-ai/bark' and 'coqui/xtts'. Please specify the precise owner/model so I can inspect their schematics thoroughly!

---

**👤 You:**
> "Cancel the prediction that has the ID `p_abc123`."

**🤖 AI Agent:**
> I immediately routed the termination request using the tool `cancel_prediction` targeted at your specified iteration ID `p_abc123`. The model sequence is permanently halted, halting processing instantly.


## Installation & Usage

To install and use the **Replicate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replicate](https://vinkius.com/mcp/replicate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
