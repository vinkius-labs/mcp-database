# Replicate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/replicate-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Run ML models via Replicate — generate images, text, audio and video from community models, track predictions and explore collections from any AI agent.

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


## Available Tools (12)
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
- **cancel_prediction**: Provide the prediction ID. The prediction status will change to "canceled".

Cancel a running prediction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Replicate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all text-to-image collections on Replicate."

**🤖 AI Agent:**
> Found the 'text-to-image' collection with featured models including stability-ai/sdxl, black-forest-labs/flux-schnell, and ideogram-ai/ideogram-v2. The collection has 50+ models total.

---

**👤 You:**
> "Search for LLM models on Replicate."

**🤖 AI Agent:**
> Found popular LLM models: meta/meta-llama-3-70b-instruct (2M+ runs), mistralai/mistral-7b-instruct-v0.3 (1.5M+ runs), google/gemma-2-27b-it (800K+ runs). Each model shows hardware requirements and example inputs.

---

**👤 You:**
> "Create a prediction using stability-ai/sdxl with prompt 'a sunset over mountains, photorealistic'."

**🤖 AI Agent:**
> Created prediction pred_abc123. Status: starting. Check back with `get_prediction` to retrieve the generated image URL once it completes (usually 10-30 seconds).


## ❓ FAQ

**Q: How do I get a Replicate API token?**
Log in to the [**Replicate API Tokens page**](https://replicate.com/account/api-tokens) and click **Create API Token**. Copy the token immediately — it starts with `r8_` and won't be shown again.

**Q: How do I run a model prediction?**
Use `create_prediction` with the model slug (e.g. "stability-ai/sdxl") and an input JSON object matching the model's schema. The prediction starts as 'starting', then 'processing', and finally 'succeeded' with output URLs. Use `get_prediction` to check status and retrieve results.

**Q: How do I find models for specific tasks?**
Use `search_models` with a query like 'text-to-image', 'llm', 'music-generation' or 'video-generation'. You can also use `list_collections` to browse curated collections by category, and `get_collection` to see featured models in each collection.

**Q: Can I cancel a running prediction?**
Yes! Use `cancel_prediction` with the prediction ID. This works for predictions that are 'starting' or 'processing'. The status will change to 'canceled' and you won't be charged for the full compute time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replicate-alternative](https://vinkius.com/mcp/replicate-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Replicate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `replicate-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Replicate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "replicate-alternative": {
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
