# Replicate MCP Server

Run ML models via Replicate — generate images, text, audio and video from community models, track predictions and explore collections from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/replicate-alternative)

## Overview
**Category:** ai-frontier
**Tools Count:** 12

## Description
Connect your **Replicate** account to any AI agent and run thousands of open-source ML models through natural conversation.

### What you can do

- **Model Discovery** — Browse, search and inspect thousands of ML models with their descriptions, run counts and hardware requirements
- **Predictions** — Run models by creating predictions and tracking their status (starting, processing, succeeded, failed)
- **Collections** — Explore curated collections of models by category (text-to-image, LLMs, audio, video)
- **Hardware Options** — View available GPU types and pricing for model inference
- **Account Info** — Check your account details and usage

### How it works

1. Subscribe to this server
2. Enter your Replicate API Token
3. Start running ML models from Claude, Cursor, or any MCP-compatible client

No more navigating the Replicate website to find models or check prediction status. Your AI acts as a dedicated ML operations assistant.

### Who is this for?

- **Developers** — quickly run image generation, text models and other ML predictions via conversation
- **ML Engineers** — discover models, compare hardware requirements and track prediction history
- **Researchers** — explore model collections, inspect version schemas and test models before deployment


## Available Tools
- **cancel_prediction**: Provide the prediction ID. The prediction status will change to "canceled".

Cancel a running prediction
- **create_prediction**: Requires the model slug in "owner/name" format and an input object matching the model's schema. Optionally specify a version ID and webhook URL. Returns the prediction object with its ID, status (starting, processing, succeeded, failed, canceled) and output. Use get_prediction to check status and retrieve results.

Run a model prediction on Replicate
- **get_account**: Returns account type, username and usage info. Use this to verify your API token is working correctly.

Get the authenticated Replicate account info
- **get_collection**: Provide the collection slug (e.g. "text-to-image", "large-language-models").

Get details for a specific model collection
- **get_model**: Provide the model slug in "owner/name" format (e.g. "stability-ai/sdxl" or "meta/meta-llama-3-70b-instruct").

Get details for a specific Replicate model
- **get_model_versions**: Each version includes its ID (64-char hash), creation date, input/output schema and cog version. Use this to find the correct version ID when creating predictions for models that require a specific version.

Get all versions of a Replicate model
- **get_prediction**: Returns the prediction ID, status (starting, processing, succeeded, failed, canceled), input, output URLs, creation time and logs. Use the prediction ID returned from create_prediction.

Get the status and result of a prediction
- **list_collections**: Collections group related models by category (e.g. "text-to-image", "large-language-models", "audio-to-audio", "image-to-video"). Each collection includes its slug, name, description and featured models.

List model collections on Replicate
- **list_hardware**: Each hardware option includes its SKU name, pricing and specifications. Useful for choosing the right GPU for your prediction workload.

List available GPU hardware on Replicate
- **list_models**: Each model includes its name, owner, description, run count, hardware requirements and cover image URL. Use this to discover available models for running predictions.

List available ML models on Replicate
- **list_predictions**: Each prediction includes its ID, model, status, creation time and output URLs. Useful for tracking prediction history and monitoring model usage.

List recent predictions on Replicate
- **search_models**: Returns models with their name, owner, description, run count and hardware. Useful for finding specific types of models (e.g. "text-to-image", "llm", "music-generation").

Search for models on Replicate by query


## Installation & Usage

To install and use the **Replicate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replicate-alternative](https://vinkius.com/mcp/replicate-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
