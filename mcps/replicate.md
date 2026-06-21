# Replicate MCP Server

Equip your AI to dynamically search, run, and monitor thousands of open-source machine learning models hosted on Replicate via simple text commands.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/replicate)

## Overview
**Category:** superpower
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Replicate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replicate](https://vinkius.com/mcp/replicate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
