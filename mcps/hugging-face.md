# Hugging Face MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hugging-face)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hugging-face-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hugging-face-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Explore AI models, datasets and Spaces via Hugging Face — search models, inspect files, review discussions and track collections from any AI agent.

## Description
Connect your **Hugging Face** account to any AI agent and explore the world's largest AI model hub through natural conversation.

### What you can do

- **Model Discovery** — Search and browse thousands of models by name, task type, framework and author
- **Model Inspection** — View model metadata including pipeline task, tags, download counts, likes and file structure
- **Dataset Exploration** — Find and inspect datasets with their descriptions, sizes and file trees
- **Spaces Gallery** — Browse ML demo apps (Gradio, Streamlit, Docker) and check their runtime status
- **Collections** — View curated collections of models, datasets and spaces organized by topic
- **Community Discussions** — Read model discussion threads for bug reports, feature requests and usage tips
- **File Tree Browsing** — List repository files (model weights, configs, tokenizers) without downloading

### How it works

1. Subscribe to this server
2. Enter your Hugging Face Access Token
3. Start exploring the ML hub from Claude, Cursor, or any MCP-compatible client

No more switching to the browser to check model tags or browse discussion threads. Your AI acts as a dedicated ML researcher.

### Who is this for?

- **ML Engineers** — quickly find models by task type, inspect their tags and file structure, and review community discussions before integration
- **Researchers** — browse datasets, explore collections and discover related models without leaving your notebook
- **Developers** — check Space runtime status, review model files and find suitable models for your application via conversation


## Available Tools
- **list_dataset_files**: Returns filenames (e.g. "train.parquet", "test.parquet", "data/", "README.md"). Optionally set a subdirectory path. Useful for understanding dataset structure before downloading.

List files in a Hugging Face dataset repository
- **create_discussion**: Requires the repo type (model, dataset or space), the repo ID in "author/name" format and the discussion title. Returns the created discussion with its ID, title and URL.

Create a new discussion on a Hugging Face repo
- **get_collection**: Provide the collection slug.

Get details for a specific Hugging Face collection
- **get_model**: Provide the model ID in "author/name" format (e.g. "google-bert/bert-base-uncased").

Get details for a specific Hugging Face model
- **get_model_tags**: Tags include framework (pytorch, tensorflow), license, dataset, language and task-specific labels. The pipeline_tag indicates the model's primary task (e.g. "text-generation", "image-classification", "translation").

Get tags and pipeline info for a Hugging Face model
- **get_space**: Provide the space ID in "author/name" format.

Get details for a specific Hugging Face Space
- **list_collections**: Optionally filter by author and limit. Returns collection slug, title, description, author, item count and likes count.

List collections on Hugging Face Hub
- **list_datasets**: Optionally filter by search term, author and limit. Returns dataset ID, author, description, download count, likes count and creation date.

List datasets on Hugging Face Hub
- **list_model_discussions**: Returns discussion title, author, creation date, number of comments and whether it is resolved. Use this to review community feedback, bug reports and feature requests for a model.

List discussions for a Hugging Face model
- **list_model_files**: Returns filenames, file sizes and paths (e.g. "model.safetensors", "tokenizer.json", "config.json", "README.md"). Optionally set a subdirectory path to list files within a specific folder. Useful for inspecting model artifacts and understanding the repository structure.

List files in a Hugging Face model repository
- **list_models**: Optionally filter by search term (free-text across model cards), author (organization or username) and limit the number of results. Returns model ID, author, pipeline task tag, download count, likes count and creation date.

List models on Hugging Face Hub
- **list_spaces**: Optionally filter by search term, author and limit. Returns space ID, title, author, SDK (Gradio, Streamlit, Docker), likes count and creation date.

List Spaces on Hugging Face Hub
- **get_user**: Returns user name, avatar, organizations, auth type, plan and access tokens metadata. Use this to verify your token is working correctly.

Get the authenticated Hugging Face user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hugging Face** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find popular text generation models with over 1000 likes."

**🤖 AI Agent:**
> Here are top text-generation models by likes: meta-llama/Llama-3.1-70B (45k likes), mistralai/Mixtral-8x7B (12k likes), microsoft/Phi-3-mini (8k likes) and google/gemma-2-9b (6k likes). Would you like the file structure for any of these?

---

**👤 You:**
> "Show me what files are in the bert-base-uncased model."

**🤖 AI Agent:**
> The bert-base-uncased repo contains: config.json (443 bytes), pytorch_model.bin (440 MB), tf_model.h5 (440 MB), flax_model.msgpack (440 MB), tokenizer.json (466 KB), tokenizer_config.json (48 bytes), vocab.txt (232 KB) and README.md. It has weights in PyTorch, TensorFlow and Flax formats.

---

**👤 You:**
> "What discussions are happening on the Llama-3 model page?"

**🤖 AI Agent:**
> There are 23 active discussions on meta-llama/Llama-3-8B. Top threads include: 'Fine-tuning with PEFT/LoRA — memory requirements' (18 replies), 'Quantization to 4-bit — GGUF format' (14 replies) and 'Comparison with Mistral-7B on reasoning tasks' (9 replies).


## Installation & Usage

To install and use the **Hugging Face** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hugging-face](https://vinkius.com/mcp/hugging-face)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
